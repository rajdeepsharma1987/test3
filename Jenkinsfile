
pipeline {
  agent any

  stages {
    stage('Checkout Code') {
      steps {
        git branch: 'main', url: 'https://github.com/rajdeepsharma1987/test3.git'
      }
    }

    stage('Build') {
      steps {
        echo 'Static website hai — build ki zarurat nahi.'
      }
    }

    stage('Run Website') {
      steps {
        echo 'Starting local web server...'
        // simple python server for local run
        bat 'python -m http.server 8081'
      }
    }
  }
}
    
