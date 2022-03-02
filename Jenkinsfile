
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
        mvn clean install
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
        sh '''
          docker cp /root/workspace/MiriamFolder/MiriamPipeline/target/sparkjava-hello-world-1.0.war tomcat://usr/local/tomcat/webapps
        '''
      }
    }
  }
}
