pipeline{
    agent any
    stages {
        stage("Checkout"){
            steps{
                echo "Git checkout"
                git 'https://github.com/Praveen-66/Pipeline.git'
            }
        }
        stage("Build"){
            steps{
                echo "Building..."
                bat 'build.bat'
            }
        }
        stage("Test"){
            steps{
                echo "Testing..."
                bat 'test.bat'
            }
        }
        stage("Deploy"){
            steps{
                echo "Deploying..."
                bat 'deploy.bat'
            }
        }
    }
    
}
