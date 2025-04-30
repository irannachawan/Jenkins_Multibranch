pipeline{
    agent any
    parameters {
        choice (name: 'select environment', choices: ['main', 'Dev', 'Staging'])
    }
    stages{
        stage('Checkout'){
            steps{
                echo"Checking SCM repository"
            }
        }

        stage('Build'){
            when {
                branch 'main' 
            }
            steps{
                echo"Building the artifact"
            }
        }
        stage('Test'){
            parallel{
                stage('Test1'){
                    steps{
                echo"Test 1 under progress"
                    }
                }

                stage('Test2'){
                    steps{
                echo"Test 2 under progress"
                    }
                }

               
            }
            
        }
        stage('Deploy'){
            steps{
                echo"Deploying the build"
            }
        }
                    
    }
}