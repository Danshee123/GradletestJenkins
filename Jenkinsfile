pipeline {
    agent any
    stages {
        stage('Gradle') {
            steps {
                bat 'gradle --version'
            }
        }
        stage('Building') {

            node{ 
                if(isUnix()){
                    sh 'gradle build --info'
                }
                else{
                    bat 'gradle build --info'
                }
            }
        }
    }
}