pipeline {
  agent {
    node {
      label 'docker'
    }

  }
  stages {
    stage('Parallel') {
      parallel {
        stage('Parallel') {
          steps {
            echo 'para'
          }
        }

        stage('Test') {
          steps {
            echo 'test'
          }
        }

      }
    }

    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Builb'
          }
        }

        stage('Run') {
          steps {
            echo 'run'
          }
        }

      }
    }

    stage('Clean') {
      steps {
        echo 'clean'
      }
    }

  }
}