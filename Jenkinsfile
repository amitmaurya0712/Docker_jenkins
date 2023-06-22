pipeline{
    agent any
    stages{
        stage("Checkout"){
            steps{
                git branch: 'main', url: 'https://github.com/amitmaurya0712/Docker_jenkins.git'
            }
        }
    }

    stages{
        stage("Docker Build"){
            steps{
                sh 'docker build -t amimau:1 .'
            }
        }
    }
}