pipeline {
    agent any
    environment {
        JAVA_HOME = 'C:\Program Files\Java\jdk-17'
        PYTHON_HOME = 'C:\Users\hug17\AppData\Local\Programs\Python\Python313'
        PATH = "${env.PATH};${JAVA_HOME}\\bin;${PYTHON_HOME}"
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
