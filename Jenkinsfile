pipeline{
    agent none
    stages{
        stage("Checkout"){
            steps{
                git branch: 'main', url: 'https://github.com/amitmaurya0712/Docker_jenkins.git'
            }
        }
        // stage('Initialize'){
        //     def dockerHome = tool 'docker'
        //     env.PATH = "${dockerHome}/bin:${env.PATH}"
        // }

        stage("Docker Build"){
            steps{
                sh 'docker build -t amimau:1 .'
            }
        }
    }    
}