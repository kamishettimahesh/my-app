pipeline{
    agent any 
    stages{
        stage("SCM Checkout"){
            steps{
                git credentialsId: 'github', 
                url: 'https://github.com/jagadeesh-nani/my-app.git'
            }
        }
        stage("Maven Build"){
            steps{
                sh 'mvn clean package'
            }
        }
    }
}
