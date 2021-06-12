pipeline {
  agent any
  
  tools {nodejs "node - latest"}
  
  stages {
    stage('Build') {
      steps {
        bat 'npm install' 
      }
    }
    stage('Test') {
      steps {
        bat 'npm test' 
      }
    }

  }
}
