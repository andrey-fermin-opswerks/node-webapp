pipeline {
    agent { label 'linux-node' }

    stages {
        stage('Build') {
            steps {
                sh 'docker build -t $node_BUILD_NUMBER .'
                sh 'docker run $node_BUILD_NUMBER'
              
            }
        }
    }
}
