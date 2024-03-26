pipeline {
    agent any
    
    stages {
        stage('Update System') {
            steps {
                sh 'sudo yum update -y'
            }
        }
        stage('Install Httpd') {
            steps {
                sh 'sudo yum install httpd -y'
            }
        }
        stage('Start Httpd') {
            steps {
                sh 'sudo systemctl start httpd'
            }
        }
        stage('Check Httpd Status') {
            steps {
                sh 'sudo systemctl status httpd'
            }
        }
        stage('Result Test Page') {
            steps {
                echo 'Test page result'
                // You can add further steps here to verify the test page.
            }
        }
    }
}
