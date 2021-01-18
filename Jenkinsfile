pipeline {
    agent any    
    stages {
        stage('Build') {
            steps {
                bat 'npm install'
				bat 'ng build'
            }
        }
        stage('Test') {
            steps {
                bat 'ng test --browsers ChromeHeadless --watch=false'
				bat 'ng e2e'				
            }
        }
        stage('Deploy') {
            steps {
                echo 'deploying.....!!!'
            }
        }
    }
}