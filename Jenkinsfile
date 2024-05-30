pipeline {
    agent any
    stages {
        stage ('init') {
            steps {
                echo 'init stage'
            }
        }
        stage ('run') {
            steps {
                sh 'python3 /var/lib/jenkins/workspace/jenkins_pytest_pipeline/main.py'
            }
        }
        stage ('test') {
            steps {
                sh 'python3 -m pytest /var/lib/jenkins/workspace/jenkins_pytest_pipeline/test/'
            }
        }
    }
}
