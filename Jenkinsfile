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
                sh '/var/lib/jenkins/workspace/jenkins_pytest_pipeline/python3 main.py'
            }
        }
        stage ('test') {
            steps {
                sh '/var/lib/jenkins/workspace/jenkins_pytest_pipeline/python3 -m pytest test/'
            }
        }
    }
}
