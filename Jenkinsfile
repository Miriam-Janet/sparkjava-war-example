
pipeline {
  agent { label 'nodoMiriam' }
  stages {
    stage('Build') {
      steps {
        sh '''
        ls
        pwd
        echo "Buenos dias"
        docker ps
        echo "Do something"
        '''
      }
    }
    stage('Test') {
      steps {
        echo "Do something"
      }
    }
    stage('Deploy') {
      steps {
        echo "Do something"
      }
    }
  }
}
