#!groovy
@Library('jenkins-pipeline-shared@master') _

import groovy.time.TimeCategory 
import groovy.time.TimeDuration

times = [:] 


pipeline {
    agent any 
  tools {nodejs "node"}
  stage {
    stage ('install') {
      steps {
        sh 'npm install --loglevel verbose'
      }
    }
    stage ('build') {
      steps {
        sh 'npm run ng build --prod'
      }
    }
  }
