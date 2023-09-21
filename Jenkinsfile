pipeline {
  agent any
  stages {
    stage('stage1') {
      parallel {
        stage('stage1') {
          steps {
            echo 'hola mundo 1'
          }
        }

        stage('stage2') {
          steps {
            sh 'sleep 4'
            sh 'echo "jojojo"'
          }
        }

        stage('stage3') {
          steps {
            echo 'hola mundo 3'
            sh 'echo "stage 3 finish"'
          }
        }

      }
    }

  }
}