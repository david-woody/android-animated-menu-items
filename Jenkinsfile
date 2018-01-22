pipeline {
  agent {
    // Run on a build agent where we have the Android SDK installed
    label 'android'
  }
  tools {
    gradle 'Gradle2.3'
  }
  
 options {
    // Stop the build early in case of compile or test failures
    skipStagesAfterUnstable()
  }
   //定义mvn环境
  stages {
    stage('Compile') {
      steps {
        // Compile the app and its dependencies
        sh './gradlew compileDebugSources'
      }
    }
  
    stage('init') {
      steps {
        sh "gradle --version"
      }
    }
    
  }
}
