pipeline {
  agent any
  
  tools {nodejs "node - latest"}
  
  stages {
    stage('Build') {
      steps {
        bat 'npm install'
        bat 'npm build'
      }
    }
    stage('Test') {
      steps {
        bat 'CI=true npm test'
      }
    }

  }
}
