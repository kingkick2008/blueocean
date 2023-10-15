pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build Step'
        retry(count: 3)
        sh 'wqqwqwqwqw'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Test Step'
          }
        }

        stage('Test 2') {
          steps {
            echo 'Test 2'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        input(message: 'Are you sure to deploy', ok: 'Yes I m sure')
        echo 'Deploy Step'
      }
    }

    stage('Notify ') {
      steps {
        echo 'New build completed'
      }
    }

  }
}