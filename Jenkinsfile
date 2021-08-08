pipeline {
  agent any 
  tools { nodejs "node" }
  stages {
    stage ('install') {
      steps {
        sh 'npm install -g @angular/cli@9.1.0 & npm install '
      }
    }
    stage ('build') {
      steps {
        sh 'npm run ng build --prod'
      }
    }
  }
