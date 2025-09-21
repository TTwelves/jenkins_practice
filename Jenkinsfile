pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                echo 'Building Stage'
                sh 'ls -la'
            }
        }
        stage('Test'){
            steps{
                echo 'Testing Stage'
            }
        }
        stage('Deploy'){
            steps{
                echo 'Deploying'
            }
        }
    }
}