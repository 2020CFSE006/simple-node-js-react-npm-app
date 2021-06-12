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
         powershell returnStdout: true, script: '($env:CI = "true") -and (npm test)'
      }
    }

  }
}
