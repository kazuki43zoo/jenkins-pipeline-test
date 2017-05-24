pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'build artifact.'
      }
    }
    stage('unit-test') {
      steps {       
        echo 'perform unit test.'
      }
    }
    stage('integration-test') {
      steps {
        echo 'perform integration test.'
      }
    }
    stage('deploy') {
      steps {
        echo 'deploy artifact.'
      }
    }
  }
}
