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
                sh '/Users/tanhongyu/miniforge3/envs/jenkins_py/bin/python main.py'
            }
        }
        stage ('test') {
            steps {
                sh '/Users/tanhongyu/miniforge3/envs/jenkins_py/bin/python -m pytest test/'
            }
        }
    }
}