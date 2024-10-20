pipeline {
    agent any

    stages {
        stages {}
            stage('Install Node.js') {
                steps {
                   bat 'npm install'
                }
            }
            stage('Run Tests') {
                steps {
                    bat 'npm test'
                }
            }
    }
    
}
