pipeline {
    agent any 
    stages {
        stage('clone repo and clean it') { 
            steps {
                sh "https://github.com/satish1yadav1/Pipeline.git"
                sh "mvn clean -f Pipeline"
            }
        }
        stage('Test') { 
            steps {
                sh "mvn test -f Pipeline" 
            }
        }
        stage('Deploy') { 
            steps {
                sh "mvn package -f Pipelne 
            }
        }
    }
}
