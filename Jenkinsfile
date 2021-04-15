pipeline {
  agent {
    node {label 'slave'}
  }
  environment{
    BUILD_TIME=sh(script: 'date "+%y%m%d-%H%M%S"', returnStdout:true).trim()
    Work_dir=sh(script: 'PWD', returnStdout:true).trim()
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
    
      steps {
        sh 'echo $PWD'
        echo "pwd=${Work_dir}"
      }
    } 
  }
}
