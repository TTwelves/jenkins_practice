pipeline{
    agent any
    stages{
            stage('Install Dependencies'){
            steps{
            echo 'Installing Dependencies'
                sh 'pip install pytest'
            }
        }
        stage('Run Tests'){
            steps{
                sh 'pytest --junitxml=report.xml'
            }
        }
    post{
    always{
            junit 'report.xml'
            }
    }
}