def registry = 'https://valaxy057.jfrog.io//'
def imageName = 'valaxy057.jfrog.io/valaxy-docker-local/ttrend'
def version   = '2.1.2

pipeline {
    agent {
        node {
            label 'maven'
        }
    }
environment {
    PATH = "/opt/apache-maven-3.9.6/bin:$PATH"
    
}
   stages {
        stage("build"){
            steps {
                 echo "----------- build started ----------"
                sh 'mvn clean deploy -Dmaven.test.skip=true'
                 echo "----------- build complted ----------"
            }
        }
}
}

