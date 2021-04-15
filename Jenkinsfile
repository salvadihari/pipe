pipeline {
  agent {
    node {label 'slave'}
  }
  
  parameters{
    
    string (name: 'DEPLOY_ENV', defaultValue: 'TESTING', description: 'The target environment')
  }
}
