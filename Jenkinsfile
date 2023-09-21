pipeline {
  agent any
  stages {
    stage('stage1') {
      parallel {
        stage('stage1') {
          steps {
            echo 'hola mundo 1'
            sh '''touch ./paco.txt





'''
            sh 'echo "joputa" > paco.txt'
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
            archiveArtifacts(artifacts: '*.txt', allowEmptyArchive: true, fingerprint: true)
            sh 'echo $NOMBRE'
          }
        }

      }
    }

    stage('stageeee2') {
      steps {
        sh 'echo "hola 2"'
      }
    }

  }
  environment {
    NOMBRE = 'Paco'
  }
}