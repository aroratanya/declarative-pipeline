pipeline {
  agent any
  stages {
    stage('Build') {
      agent any
      environment {
        LOG_LEVEL='INFO'
      steps {
        echo 'Building Release ${RELEASE} with log level ${LOG_LEVEL}..'
      }
    }
    stage('Test') {
     
      steps {
        echo 'Testing Release ${RELEASE} but log level ${LOG_LEVEL} is not visible'
      }
    }
    

  }
  environment {
   RELEASE ='20.05'
  }
}
