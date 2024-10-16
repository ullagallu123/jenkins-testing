pipeline {
    agent {
        label 'siva'
    }
    stages {
        stage("Greeting") {
            steps {
                echo "Hello Welcome to Jenkins!"
            }
        }
    }
    post {
        always {
            cleanWs()
        }
    }
}
