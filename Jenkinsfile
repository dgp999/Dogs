pipeline{
    agent any
    stages{
        stage("Git SCM"){
            steps{
                git 'https://github.com/dgp999/declarativepipe.git'
            }
        }
        stage("Maven Build"){
            steps{
                sh "mvn clean package"
                sh "mv target/*.war target/myweb.war"
            }
        }
