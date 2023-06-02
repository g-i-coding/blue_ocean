pipeline {
  agent {
    node {
      label 'docker'
    }

  }
  stages {
    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Testing'
          }
        }

        stage('Parallel') {
          steps {
            echo 'parallel print'
          }
        }

      }
    }

    stage('Build') {
      steps {
        echo 'build'
      }
    }

    stage('clean up') {
      steps {
        echo 'cleaning up'
      }
    }

  }
}