pipeline {
  agent any
  stages {
    stage('Verify Tools') {
      parallel {
        stage('gradle') {
          steps {
            sh 'gradle -v'
          }
        }
      }
    }
    stage('Clean') {
      steps {
        sh 'gradle clean'
      }
    }
  }
  tools {
    gradle 'Gradle2.3'
  }
}