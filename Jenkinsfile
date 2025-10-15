pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/rajdeepsharma1987/test3.git'
            }
        }
        stage('Validate Files') {
            steps {
                echo '✅ Checking HTML, CSS, and JS files...'
                bat 'dir'  // instead of sh 'ls'
            }
        }
        stage('Archive Website') {
            steps {
                bat 'echo Archiving site...'
            }
        }
    }
    post {
        failure {
            echo '❌ Build failed. Please check console logs.'
        }
    }
}
