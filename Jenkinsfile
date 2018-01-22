pipeline {
  agent any
   //定义mvn环境
  def gradleHome = tool 'Gradle2.3'
  env.PATH = "${gradleHome}/bin:${env.PATH}"
  stages {
    stage('init') {
      steps {
        sh 'chmod +x gralew'
      }
    }
  }
}