pipeline {
  agent {
    node {label 'slave'}
  }
  environment{
    REPO_URL="https://github.com/salvadihari/pipe.git"
  }
  
  
  parameters{
    string (name: 'DEPLOY_ENV', defaultValue: 'TESTING', description: 'The target environment')
  }
  
  stages {
    stage('SCM Checkout'){  
      steps{
        sh 'java -version'
      }
    }
  }
}
