pipeline {
    agent { docker { image 'python:3.5.1' } }
    stages {
        stage('build') {
            steps {
                sh 'python3 helloworld.py'
                sh 'ls -lah'
                sh 'pwd'
                sh 'echo "wassup 3rd step"'
            }
        }
    }
    post {
      always {
        archiveArtifacts artifacts: 'README', fingerprint: true
      }
    }
}
