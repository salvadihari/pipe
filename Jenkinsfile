pipeline {
  agent {
    node {label 'slave'}
  }
  environment{
    BUILD_TIME=sh(script: 'date "+%y%m%d-%H%M%S"', returnStdout:true).trim()
    REPO_URL="https://github.com/salvadihari/pipe.git"
  }
  
  
  parameters{
       choice( name: 'Deploy_Env', choices: ['TESTING', 'STAGING', 'PRODUCTION'], description: 'The target environment')
  }                   
  
  
  stages {
    stage('SCM Checkout'){  
      steps{
        sh 'java -version'
      }
    }
   steps {
        sh 'env'
        sh 'echo $PWD'
    } 
  }
}
