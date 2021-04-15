pipeline {
  agent {
    node {label 'slave'}
  }
  environment{
    REPO_URL="https://github.com/salvadihari/pipe.git"
  }
  
  
  parameters{
    choices (name: 'DEPLOY_ENV', defaultValue: 'TESTING', 'Dev','Prod', description: 'The target environment')
    
  }
  
  stages {
    stage('SCM Checkout'){  
      steps{
        sh 'java -version'
      }
    }
  }
}
