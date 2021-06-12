pipeline {
  agent any
  
  tools {nodejs "node - latest"}
  
  stages {
    stage('Build') {
      steps {
        bat 'npm install'
        bat 'set CI=true&&npm run build'
      }
    }
    stage('Test') {
      steps {
        ps './jenkins/scripts/test.ps1'
      }
    }

  }
}
