pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'mvn clean install' // Example command to build the project
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test' // Example command to run tests
            }
        }
        stage('Deploy') {
            steps {
                sh 'docker build -t my-image .' // Example command to build a Docker image
                sh 'docker push my-image' // Example command to push the image to a registry
            }
        }
    }
}
