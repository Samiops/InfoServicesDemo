pipeline {
  agent none
  stages {
    stage('Maven Latest Stage') {
      agent {
        docker { image 'maven:latest' }
      }
      steps {
        sh 'mvn --version'
      }
    }
    stage('Maven IBM Java Stage') {
      agent {
        docker { image 'maven:ibmjava' }
      }
      steps {
        sh 'mvn --version'
      }
    }
  }
}
