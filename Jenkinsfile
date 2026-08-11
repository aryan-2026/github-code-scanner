pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Test Jenkins') {
            steps {
                bat 'echo "Jenkins is working!"'
            }
        }
    }
}
