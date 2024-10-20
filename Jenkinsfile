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
            stage('Approval for Production Deployment') {
            steps {
                    // Approval step: Pause for manual input
                    input(message: 'Do you want to proceed with deployment to production?', ok: 'Deploy')
                }
            }
        }
            stage('Deploy to Production') {
                steps {
                    echo 'Deploy to production'
                }
            }
        
    
}
