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
            echo 'hola mundo 2'
          }
        }

        stage('stage3') {
          steps {
            echo 'hola mundo 3'
          }
        }

      }
    }

  }
}