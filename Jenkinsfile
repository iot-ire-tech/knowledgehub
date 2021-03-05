pipeline {
  environment {
    registry = "tonyennis/sandbox"
    registryCredential = 'credentials-id-tonyennis'
  }
  agent any
  stages {
    stage('Building image') {
      steps{
        script {
          docker.build registry + ":$BUILD_NUMBER"
        }
      }
    }
  }
}

