pipeline {
    agent {
        label 'master'
    }
    stages {
        stage('MAKEDIRECTORY') {
            steps {
                sh """
                mkdir /tmp/pipedir4
                """
            }
        }
        
        stage('TOUCH NEW FILE') {
            steps {
                sh """
                touch /tmp/pipefile3
                """
            }
        }
        
        stage('COPY FILE TO DIR') {
            steps {
                sh """
                cp /tmp/pipefile3 /tmp/pipedir4
                """
            }
        }
    }
}
