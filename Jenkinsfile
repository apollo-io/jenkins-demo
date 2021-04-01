pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Compiling code, building, unit test, packaging'
      }
    }

    stage('Acceptance') {
      steps {
        echo 'Deploy to CI, run acceptance tests'
      }
    }

    stage('Staging') {
      steps {
        sh 'Check dependency versions on SIT, deploy to SIT, run acceptance tests on SIT'
      }
    }

  }
}