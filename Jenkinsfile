pipeline {
    agent {
        docker { 'python:2.7-alpine' }
    stages{
        stage("build") {
            steps {
                sh """
                    docker build -t hello_there .
                """
            }
        }
        stage("run") {
            steps {
                sh """
                    docker run --rm hello_there
                """
            }
        }
    }
}
