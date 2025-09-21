pipeline{
    agent any
    stages{
            stage('Install Dependencies'){
            steps{
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