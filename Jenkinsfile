pipeline {
    agent {
        docker { image ‘maven:3.5.2’ }
    }
    stages {
        stage('Test') {
            steps {
                sh ‘mvn --version'
            }
        }
    }
}