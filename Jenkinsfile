pipeline {
    agent any  // Run on any available Jenkins agent

    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main', url: 'https://Yeshankroy/todo-cicd'
            }
        }

        stage('Build') {
            steps {
                echo '🔨 Building the project...'
                // If it's a .NET project, use:
                // bat 'msbuild Project.sln /p:Configuration=Release'
            }
        }

        stage('Test') {
            steps {
                echo '🧪 Running tests...'
                // Add test commands here, e.g., NUnit for .NET
            }
        }

        stage('Deploy') {
            steps {
                echo '🚀 Deploying to server...'
                // Add deployment commands
            }
        }
    }
}
