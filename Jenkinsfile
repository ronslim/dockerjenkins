pipeline {
    agent {
        docker { image 'httpd:2.4.57-alpine' }
    }
    stages {
        stage('Docker Test') {
            steps {
                echo 'Docker Run Test'
                sh "docker run -d -p 8085:80 -v $(which docker):/usr/bin/docker -v /var/run/docker.sock:/var/run/docker.sock httpd:2.4.57-alpine"
            }
        }
    }
}
