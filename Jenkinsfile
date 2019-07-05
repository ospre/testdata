pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        build(job: 'bobs', quietPeriod: 1)
      }
    }
    stage('Test') {
      steps {
        junit(testResults: 'testy', allowEmptyResults: true, healthScaleFactor: 1)
      }
    }
    stage('Deploy') {
      steps {
        sh '#!'
      }
    }
  }
}