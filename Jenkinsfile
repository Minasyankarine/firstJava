pipeline {
  agent any
  stages {
    stage('stage 1') {
      steps {
        build(propagate: true, job: 'firstJava', quietPeriod: 1, wait: true)
      }
    }

  }
}