pipeline {
    agent any
    tools {
        // Install the Maven version configured as "M3" and add it to the path.
        maven 'maven'
    }
    stages {
        stage('Clean') {
            steps {
                // Get some code from a GitHub repository
                git 'https://github.com/tomlabour/GoSecuri.git'
                
                sh 'mvn clean'
            }
        }
    }
}
