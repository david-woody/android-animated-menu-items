pipeline {
  agent any
  stages {
    stage('Compile') {
      steps {
        sh './gradlew compileDebugSources'
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