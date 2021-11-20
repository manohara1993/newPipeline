pipeline {
    agent any
    
    tools{
        maven '3.8.3'
    }
    
    environment {
                SERVICE_BRANCH = "main"
            }
            
    stages {
        stage('checkout') {
            steps {
                echo "the branch is ${params.branch}"
                git branch: 'main', url: 'https://github.com/manohara1993/newPipeline.git'
                }
            }
        stage('compile and build'){
            steps{
                echo 'Success'
                echo 'Success'
                }
            }
        stage('Test'){
           
		steps{
                sh "mvn test"
             }
        }
    }
    post { 
        always { 
             echo 'Success'
        }
    }
}

