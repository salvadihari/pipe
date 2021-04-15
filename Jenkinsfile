pipeline {
  agent {
    node {label 'slave'}
  }
  environment{
    REPO_URL="https://github.com/salvadihari/pipe.git"
  }
  
  
  parameters([
       choice( name: 'Deploy_Env', choices: ['TESTING', 'STAGING', 'PRODUCTION'], description: 'The target environment')
        ])                   
  
  
  stages {
    stage('SCM Checkout'){  
      steps{
        sh 'java -version'
      }
    }
  }
}
