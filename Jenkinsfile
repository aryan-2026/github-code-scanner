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
        sh '''
            semgrep scan \
            --config auto \
            --json \
            --output semgrep-report.json .
        '''
    }
}
    }
}
