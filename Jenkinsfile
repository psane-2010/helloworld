pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'echo Build test'
            }
        }
        stage('test') {
            steps {
                sh 'python helloworld.py'
            }
        }
    }
    post {
        always {
            emailext body: 'A Test EMail',
            recipientProviders: [[$class: 'DevelopersRecipientProvider'], [$class: 'RequesterRecipientProvider']],
            subject: 'Test'
        }
    }
}