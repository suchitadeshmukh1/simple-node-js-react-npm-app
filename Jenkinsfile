pipeline {
    agent {
        podman {
            image 'registry.redhat.io/rhscl/nodejs-12-rhel7'
            args '-p 3000:3000'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
    }
}
