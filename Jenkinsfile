pipeline {
    agent any

    stages {
        stage('checkout') {
            steps {
                git branch: 'feature/christ', credentialsId: 'git-credential', url: 'https://github.com/Galiomid/commercial_card.git'
            }
        }
        stage('compile') {
            steps {
                sh "mvn compile"
            }
        }
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
    }
}
