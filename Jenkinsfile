pipeline {
    agent { docker { image 'python:3.5.1' } }
    stages {
        stage('build') {
            steps {
                sh 'python3 helloworld.py'
                sh 'ls -lah'
                sh 'echo "wassup 3rd step"'
            }
        }
    }
}
