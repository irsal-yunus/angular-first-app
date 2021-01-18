pipeline {
    agent any    
    stages {
        stage('Build') {
            steps {
                bat 'npm install'
		bat 'npm run ng -- build'
            }
        }
        stage('Test') {
            steps {
                bat 'npm run ng test --browsers ChromeHeadless --watch=false'
		bat 'npm run ng e2e'				
            }
        }
        stage('Deploy') {
            steps {
                echo 'deploying.....!!!'
            }
        }
    }
}
