pipeline {
    agent any 
    stages {
        stage('clone repo and clean it') { 
            steps {
                sh "git clone https://github.com/satish1yadav1/jenkins_pipeline.git"
                sh "mvn clean -f jenkins_pipeline"
            }
        }
        stage('Test') { 
            steps {
                sh "mvn test -f jenkins_pipeline" 
            }
        }
        stage('Deploy') { 
            steps {
                sh "mvn package -f jenkins_pipeline" 
            }
        }
    }
