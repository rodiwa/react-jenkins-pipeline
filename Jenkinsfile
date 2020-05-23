pipeline {
  agent any

  stages {
    stage('Initial') }{
      steps {
        echo 'initial step comes here'
      }
    }
    stage('Eslint') {
      step {
        echo 'eslit step comes here'
        sh 'npm run test'
      }
    }
  }
}