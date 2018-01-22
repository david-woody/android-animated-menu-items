pipeline {
  agent any
  stages {
    stage ('Verify Tools'){
      steps {
        parallel (
          gradle: { sh "npm -v" },
        )
      }
    }
    stage('Compile') {
      steps {
        sh 'gradle --version'
      }
    }
    stage('init') {
      steps {
        sh 'gradle --version'
      }
    }
  }
  tools {
    gradle 'Gradle2.3'
  }
  options {
    skipStagesAfterUnstable()
  }
}