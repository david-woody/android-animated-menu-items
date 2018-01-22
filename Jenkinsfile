pipeline {
  agent any
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