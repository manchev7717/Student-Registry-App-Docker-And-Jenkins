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
            stage('Deploy to Staging') {
                steps {
                    echo 'Deploy to staging'
                }
            }
            stage('Deploy to Production') {
                steps {
                    echo 'Deploy to production'
                }
            }
        }
    
}
