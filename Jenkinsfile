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
    post {
        always {
            echo 'One way or another, I have finished'
            deleteDir()
        }
        success {
            echo 'I succeeeded!'
        }
        unstable {
            echo 'I am unstable :/'
        }
        failure {
            echo 'I failed :('
        }
        changed {
            echo 'Things were different before...'
        }
    }
}