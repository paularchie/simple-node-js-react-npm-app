pipeline {
        agent {
            label 'docker' 
        }
        stages {
            stage('Build') {
                agent {
                    docker {
                    // Set both label and image
                    label 'docker'
                    image 'node:6-alpine'
                        args '-p 3000:3000'
                    }
             }
            steps {
                sh 'npm install'
            }
            }
        }
}
