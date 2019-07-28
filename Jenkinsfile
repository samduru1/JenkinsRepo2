pipeline {
    agent {
        label 'master'
    }
    stages {
        stage('MAKEDIRECTORY') {
            steps {
                sh """
                mkdir /tmp/pipedir3
                """
            }
        }
        
        stage('TOUCH NEW FILE') {
            steps {
                sh """
                touch /tmp/pipefile2
                """
            }
        }
        
        stage('COPY FILE TO DIR') {
            steps {
                sh """
                cp /tmp/pipefile2 /tmp/pipedir3
                """
            }
        }
    }
}
