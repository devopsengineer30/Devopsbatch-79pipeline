pipeline {
  agent any
  stages {
    stage('Dev') {
      steps {
        echo 'This is dev stage'
      }
    }

    stage('Build') {
      steps {
        echo 'This is build stage'
      }
    }

    stage('Test') {
      steps {
        echo 'This is test stage'
      }
    }

    stage('UAT') {
      parallel {
        stage('UAT') {
          steps {
            echo 'This is UAT Stage'
          }
        }

        stage('Deploy') {
          steps {
            echo 'This is deploy Stage'
          }
        }

        stage('Operate') {
          steps {
            echo 'This is operate stage'
          }
        }

      }
    }

  }
}