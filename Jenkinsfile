pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''pwd
ls
ll
ifconfig'''
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'teststep'
          }
        }

        stage('tes par') {
          steps {
            echo 'test par'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploy'
      }
    }

  }
}