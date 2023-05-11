pipeline {
    agent any
    stages {
        stage('Build'){
            steps {
                sh "docker prune -y"
              }
        }

        stage('Test'){
            steps {
                sh "docker run -d -p 5000:5000 slstef/jenkinslab4:latest"
              }
        }

        stage('Deploy'){
            steps {
                sh "ls -la"
		sh "docker ps"
              }
        }
    }
}
