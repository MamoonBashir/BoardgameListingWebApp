pipeline {
    agent any

    stages {
        stage('Git Checkout') {
            steps {
              git  'https://github.com/MamoonBashir/BoardgameListingWebApp.git'
            }
        }
        
        stage('compile') {
            steps {
                sh "mvn compile"
            }
        }
        
        stage('test') {
            steps {
                sh "mvn test"
            }
        }
        
        stage('package') {
            steps {
                sh "mvn package"
            }
        }
        
        stage('Install') {
            steps {
                sh 'mvn install'
            }
        }
        
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
    }
}
