pipeline {
  agent {
    node {label 'slave'}
  }
  environment{
    REPO_URL="https://github.com/salvadihari/pipe.git"
  }
  
  
  parameters{
       choice( name: 'PARAMETER_01', choices: ['TESTING', 'STAGING', 'PRODUCTION'], description: 'The target environment')
                           
  }
  
  stages {
    stage('SCM Checkout'){  
      steps{
        sh 'java -version'
      }
    }
  }
}
