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
        stage("Docker Version"){
            steps{
                sh"""
                docker version
                """
            }
        }
        stage("Java Version"){
            steps{
                sh"""
                java --version
                """
            }
        }
        stage("Python Version"){
            steps{
                sh"""
                python3 --version
                pip3 --version
                """
            }
        }
        stage("AWS CLI2 Version"){
            steps{
                sh"""
                aws --version
                """
            }
        }
        stage("Miscellanious Tools"){
            steps{
                sh"""
                kubectl --version --client
                terraform --version
                packer --version
                trivy --version
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
