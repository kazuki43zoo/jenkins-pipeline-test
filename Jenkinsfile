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
        parallel(
          "unit-test": {
            echo 'perform unit test.'
            
          },
          "integration-test": {
            echo 'perform integration test.'
            sh 'sh ./test.sh'
            
          }
        )
      }
    }
    stage('deploy') {
      steps {
        echo 'deploy artifact.'
      }
    }
  }
}