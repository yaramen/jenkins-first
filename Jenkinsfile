pipeline {
    stages {
        stage('build frontend') {
            agent { docker { image 'php' } }
            steps {
                sh 'php --version'
            }
        }
    }

    stages {
        stage('build backend') {
            agent { docker { image 'node' } }
            steps {
                sh 'npm --version'
            }
        }
    }
}