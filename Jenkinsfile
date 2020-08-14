pipeline {
  agent any
  stages {
    stage('echo') {
      steps {
        echo 'hello AKT'
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