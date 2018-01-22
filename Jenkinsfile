pipeline {
  agent any
   //定义mvn环境
  stages {
    def gradleHome = tool 'Gradle2.3'
    env.PATH = "${gradleHome}/bin:${env.PATH}"
  
    stage('init') {
      steps {
        sh "gradle --version"
      }
    }
    
  }
}