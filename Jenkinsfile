pipeline {
    agent any
    stages {
        stage('Gradle') {
            steps {
                bat 'gradle --version'
            }
        }
        stage('Building') {

            steps{
                    bat 'gradle build --info'
                }
            }
        }
    }