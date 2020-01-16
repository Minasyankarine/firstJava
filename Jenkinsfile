pipeline {
  agent any
  stages {
    stage('stage 1') {
      steps {
        build(propagate: true, job: 'firstJava', quietPeriod: 1, wait: true)
      }
    }

    stage('stage 2') {
      steps {
        junit(testResults: 'test', allowEmptyResults: true, healthScaleFactor: 1, keepLongStdio: true)
      }
    }

  }
}