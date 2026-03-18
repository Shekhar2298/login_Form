pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Cloning source'
            }
        }

        stage('Check Files') {
            steps {
                sh 'pwd'
                sh 'ls -la'
            }
        }

        stage('Deploy') {
            steps {
                sh 'sudo cp -r * /usr/share/nginx/html/'
                sh 'sudo systemctl restart nginx'
            }
        }
    }
}
