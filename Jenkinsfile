pipeline{
    agent any
    stages{
        stage('github'){
            steps{
                git credentialsId: 'GitHub_app', url: 'https://github.com/Sathishkumar-002/seventhproject.git'
            }
        }
        stage('test'){
            steps{
                echo "welcome to test"
            }
        }
        stage('deploy'){
            steps{
                sh 'python3 app.py'
            }
        }
    }
}
