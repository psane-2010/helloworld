pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'echo Build test'
                ansiblePlaybook colorized: true, installation: 'Ansible',playbook: '${WORKSPACE}/test.yml'
            }
        }
        stage('test') {
            steps {
                sh 'python helloworld.py'
            }
        }
    }

}