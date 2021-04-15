pipeline {
  agent {
    node {label 'slave'}
  }
  environment{
    REPO_URL="https://github.com/salvadihari/pipe.git"
  }
  
  
  parameters{
    string (name: 'DEPLOY_ENV', defaultValue: 'TESTING', 'Dev','Preprod','Prod' description: 'The target environment')
    string (name: 'DEPLOY_ENV', defaultValue: 'Dev' description: 'The target environment')
    string (name: 'DEPLOY_ENV', defaultValue: 'Preprod' description: 'The target environment')
    string (name: 'DEPLOY_ENV', defaultValue: 'Prod' description: 'The target environment')
  }
  
  stages {
    stage('SCM Checkout'){  
      steps{
        sh 'java -version'
      }
    }
  }
}
