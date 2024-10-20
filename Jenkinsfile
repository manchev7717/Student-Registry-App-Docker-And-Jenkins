pipeline {
    agent any
        stages {
            stage('NPM install') {
                steps {
                   bat 'npm install'
                }
            }
            //trigger testing
            stage('Run Tests') {
                steps {
                    bat 'npm test'
                }
            }
        }
    
}
