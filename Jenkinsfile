pipeline {
    agent any
    stages {
        stage('Docker Test') {
            steps {
                echo 'Docker Run Test'
                sh "docker run -d -p 8085:80 httpd:2.4.57-alpine"
            }
        }
    }
}
