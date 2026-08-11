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
                bat 'C:\\Python314\\Scripts\\semgrep.exe scan --config auto --json --output semgrep-report.json .'            }
        }
    }
}
