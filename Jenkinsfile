pipeline{
    agent any
    environment {
        GIT_CREDENTIALS_ID = 'Git_Pipeline'  // Add in Jenkins -> Credentials
    }
    stages{
        stage('Checkout'){
            steps{
                echo"Checking SCM repository"
            }
        }

        stage('Build'){
            steps{
                echo"Building the artifact"
            }
        }
        stage('Test'){
            steps{
                echo"Testing the build"
            }
        }
        stage('Deploy'){
            steps{
                echo"Deploying the build"
            }
        }
                    
    }
}