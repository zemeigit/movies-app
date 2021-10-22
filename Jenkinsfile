pipeline {
    agent any
    tools {nodejs "ZemeiNode"}
    stages {
        stage('Build') {
            steps {
                git 'https://github.com/zemeigit/movies-app'
                sh 'cd client'
                sh 'npm run build'
                sh 'serve -s build -p 8000'
            }
        }
    }
}