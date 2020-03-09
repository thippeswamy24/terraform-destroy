pipeline {
    agent {
        node {
            label 'master'
        }
    }

    stages {

        stage('terraform started') {
            steps {
                sh 'echo "Started...!" '
            }
        }
        stage('Destroying Services') {
            steps {
                 sh 'sudo /home/ec2-user/terraform destroy --auto-approve /home/ec2-user/newfolder'
            }
        }
