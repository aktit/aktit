pipeline {
  agent any
  stages {
    stage('echo') {
      parallel {
        stage('echo') {
          steps {
            echo 'hello AKT'
          }
        }

        stage('echo3') {
          steps {
            sh 'echo 3'
          }
        }

        stage('echo4') {
          steps {
            sh 'echo 4'
          }
        }

      }
    }

    stage('echo2') {
      steps {
        sh 'echo echo2'
      }
    }

  }
  triggers {
    githubPush()
  }
}