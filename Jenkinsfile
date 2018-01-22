pipeline {
  agent any
  stages {
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