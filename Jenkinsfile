pipeline {
    agent {label 'label1'}
    stages {
        stage('Build') {
            steps {
                    git branch: 'master', url: 'https://github.com/omkar8867/dockerfile.git'
                    sh '''
                        docker build -t my-python:1.0.0 .
                    ''' 
            }
        }
    }
}
