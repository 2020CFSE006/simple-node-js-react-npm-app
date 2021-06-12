pipeline {
  agent any
  stages {
    stage('') {
      steps {
        bat(script: 'Build', returnStatus: true, label: 'Build')
        bat(script: 'Test', label: 'Test')
      }
    }

  }
}