pipeline { 
    agent {
        label any
    }
    stages {
        stage('Lint Checks') {
            steps {
                sh "echo Performing style checks"
                sh "pip3 install pylint"
                sh "pylint payment.py || true"
            }
        }
        stage('Static Code Analysis') {
            steps {
                sh "echo Static Checks ...."
            }
        }
    }
}