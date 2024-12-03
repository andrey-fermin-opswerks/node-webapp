pipeline {
    agent { label 'linux-node' }

    stages {
        stage('Build') {
            steps {
                sh 'docker build -t node_$BUILD_NUMBER .'
                sh 'docker run node_$BUILD_NUMBER'
              
            }
        }
    }
}
