pipeline {
  agent {
    // Run on a build agent where we have the Android SDK installed
    label 'android'
  }
  
  tools {
    gradle 'Gradle2.3'
  }
  

  stages {
    stage ('Verify Tools'){
      steps {
        parallel (
          gradle: { sh "gradle -v" }
        )
      }
    }
    stage ('Clean'){
      steps {
          sh "gradle clean" 
      }
    }
    
  }
}
