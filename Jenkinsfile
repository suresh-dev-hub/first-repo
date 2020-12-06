pipeline {
  agent any
  stages {
    stage('stage1') {
      parallel {
        stage('stage1') {
          steps {
            pwd()
            sleep 5
          }
        }

        stage('stage1.2') {
          steps {
            echo 'Fetching PWD'
          }
        }

      }
    }

    stage('Stage2') {
      steps {
        echo 'Got PWD'
        sleep 5
      }
    }

  }
}