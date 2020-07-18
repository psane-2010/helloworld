pipeline {
    agent { docker: { image: 'python3.7.2' } }
    stages {
        stage('build') {
            steps {
                sh 'pip install -r requirements.txt'
            }
        }
        stage('test') {
            steps {
                sh 'python helloworld.py'
            }
        }
    }
}