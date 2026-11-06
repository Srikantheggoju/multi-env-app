pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo "Building Branch: ${env.BRANCH_NAME}"
            }
        }

        stage('Build') {
            steps {
                sh 'docker build -t multi-env-app:${BRANCH_NAME} .'
            }
        }

        stage('Test') {
            steps {
                echo 'Application Built Successfully'
            }
        }
    }
}
