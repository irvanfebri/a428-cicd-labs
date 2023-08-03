pipeline {
    agent {
        docker {
<<<<<<< HEAD
            image 'node:lts-bullseye-slim' 
            args '-p 3000:3000'
=======
            image 'node:16-buster-slim' 
            args '-p 3000:3000' 
>>>>>>> 8e18c81 (add string sleep123348e)
        }
    }
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') { 
            steps {
                sh 'npm install' 
            }
<<<<<<< HEAD
        } 
        stage('Test') {
=======
        }
        stage('Test') { 
>>>>>>> 8e18c81 (add string sleep123348e)
            steps {
                sh './jenkins/scripts/test.sh' 
            }
        }
        stage('Manual Approval') {
            input {
                message "Lanjutkan ke tahap Deploy?"
            }
            steps {
                echo "Ready to deployment"
            }
        }
        stage('Deliver') {
            steps {
<<<<<<< HEAD
                sh './jenkins/scripts/deliver.sh'
                input message: 'Finished using the web site? (Click "Proceed" to continue)'
                sh './jenkins/scripts/kill.sh'
=======
                sh './jenkins/scripts/deliver.sh' 
                sh './jenkins/scripts/kill.sh' 
>>>>>>> 8e18c81 (add string sleep123348e)
            }
        }
    }
}
