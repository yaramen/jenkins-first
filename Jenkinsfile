pipeline {
    agent none
    stages {
        stage('build frontend') {
            agent { docker { image 'php' } }
            steps {
                sh 'php --version'
            }
        }
        stage('build backend') {
            agent { docker { image 'node' } }
            steps {
                sh 'npm --version'
            }
        }
    }
}