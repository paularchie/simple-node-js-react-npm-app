pipeline {
     agent {
        label any
    }
   
    stages {
         agent {
        docker {
            image 'node:6-alpine'
            args '-p 3000:3000'
        }
    }
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
    }
}
