pipeline {
    agent { label "linux" }
    stages{
        stage("build") {
            steps {
                sh """
                    docker build -t hello_ther .
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
