pipeline {
    agent any 
  tools {nodejs "node"}
  stage {
    stage ('install') {
      steps {
        sh 'npm install '
      }
    }
    stage ('build') {
      steps {
        sh 'npm run ng build --prod'
      }
    }
  }
