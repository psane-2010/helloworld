pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'echo Build test'
                sh ansible-playbook test.yml
            }
        }
        stage('test') {
            steps {
                sh 'python helloworld.py'
            }
        }
    }

}