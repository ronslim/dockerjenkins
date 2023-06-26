pipeline {
    agent {
        docker { image 'httpd:2.4.57-alpine' }
    }
    stages {
        stage('Test') {
            steps {
                echo 'Docker Run Test'
                sh 'docker run -d -p 8085:80 httpd:2.4.57-alpine'
            }
        }
    }
}
