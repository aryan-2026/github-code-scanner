pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Security Scan') {
            steps {
                bat 'semgrep scan --config auto --json --output semgrep-report.json .'
            }
        }
    }
}
