def registry = 'https://valaxy02.jfrog.io'
def imageName = 'valaxy02.jfrog.io/valaxy-docker/ttrend'
def version   = '2.0.2'
pipeline{
    agent  any
    environment {
        PATH = "/opt/apache-maven-3.9.3/bin:$PATH"
    }
    stages {
        stage('build') {
            steps{
                echo "------------ build started ---------"
                sh 'mvn clean deploy -Dmaven.test.skip=true'
                echo "------------ build completed ---------"
        }
      }


      
    }
    }
