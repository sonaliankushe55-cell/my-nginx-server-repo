pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                git 'https://github.com/sonaliankushe55-cell/my-nginx-server-repo.git'
            }
        }

        stage('Run Ansible Playbook') {
            steps {
                sh '''
                ansible-playbook -i hosts deploy.yml
                '''
            }
        }
    }
}
