pipeline{
    
    agent any
    tools{maven 'M3'}
    
    stages{
        stage('Checkout'){
            steps{
                git branch:'main', url:'https://github.com/yadneshingole/SpringPetClinic.git'
            }
        }
        stage('Build'){
            steps{
                sh 'mvn compile'
            }
        }
        stage('Test'){
            steps{
                sh 'mvn test'
            }
        }
        stage('Package'){
            steps{
                sh 'mvn package'
            }
        }

        
    }
}
