pipeline{
    agent
    stages{
        stage('Git Clone'){
            steps{
                git 'https://github.com/ohmsmaestro/jenkins_mavenproject.git'
            }
        }
        
        stage('Maven Test'){
            steps{
                sh 'mvn test'
            }
        }
        
        stage('Maven Build'){
            steps{
                sh 'mvn package'
            }
        }
        
        stage('Maven Deploy'){
            steps{
                echo 'Deploying........'
            }
        }
    }
}
