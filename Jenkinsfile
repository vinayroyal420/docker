pipeline {
    agent { label"jdk-11"}

    stages {
        stage(docker) {
            steps {
                sh "curl -fsSL https://get.docker.com -o get-docker.sh"
                sh "sh get-docker.sh"
                sh "docker info"
                sh "docker container run hello-world"
                sh "docker container ls -al"
                /*sh "docker --version"*//
            }
        }
    }
}