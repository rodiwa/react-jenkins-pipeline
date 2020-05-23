pipeline {
  agent any

  tools {
    nodejs 'node'
  }

  stages {
    stage('Get git repo') {
      steps {
        git 'https://github.com/rodiwa/react-jenkins-pipeline'
      }
    }
    stage('Log Node version') {
      steps {
        echo 'Node version is:'
        sh 'node --version'
      }
    }
    stage('Install dependencies') {
      steps {
        echo 'Install dependencies'
        sh 'npm install'
      }
    }
    stage('Eslint') {
      steps {
        echo 'eslit step comes here'
        sh 'npm run test:noWatch'
      }
    }
    stage('Last command') {
      steps {
        echo 'if this runs, then all tests have passed'
      }
    }
  }
}
