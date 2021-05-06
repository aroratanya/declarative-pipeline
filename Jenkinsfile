pipeline {
  agent any
  stages {
    stage('Build') {
      agent any
      environment{
          LOG_LEVEL='INFO'
      }
      steps {
        echo "Building release ${RELEASE} with log level ${LOG_LEVEL} ..."
      }
    }
    stage('Test'){
      steps{
        echo "Testing release ${RELEASE} but log level ${LOG_LEVEL} is not visible..."
      }
    }
  }
  environment {
    RELEASE = '20.05'
  }
}
