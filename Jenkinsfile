pipeline {
agent { docker 'maven:3.5.2’ }
    stages {
        stage('Test') {
            steps {
                sh ‘mvn --version'
		sh ‘echo “maven version printed”’
            }
        }
    }
}