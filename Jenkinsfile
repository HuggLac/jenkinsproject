pipeline {
    agent any
    environment {
        PYTHON_HOME = 'C:\\Users\\hug17\\AppData\\Local\\Programs\\Python\\Python313'
        PATH = "${env.PATH};${PYTHON_HOME}"
    }
  
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/HuggLac/jenkinsproject.git'
            }
        }
        stage('Build') {
            steps {
                script {
					bat 'echo "Running on Windows"'
					bat 'python helloworld.py'					
                }
            }
        }
    }
}
