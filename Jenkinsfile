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
        stage("NODEJS Version"){
            steps{
                sh """
                node -v
                npm -v
                """
            }
        }
    }
    post {
        always {
            cleanWs()
        }
    }
}
