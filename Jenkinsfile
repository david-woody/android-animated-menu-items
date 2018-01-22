pipeline {
  agent {
    // Run on a build agent where we have the Android SDK installed
    label 'android'
  }
 options {
    // Stop the build early in case of compile or test failures
    skipStagesAfterUnstable()
  }
   //定义mvn环境
  stages {
    
  
    stage('init') {
    def gradleHome = tool 'Gradle2.3'
    env.PATH = "${gradleHome}/bin:${env.PATH}"
      steps {
        sh "gradle --version"
      }
    }
    
  }
}