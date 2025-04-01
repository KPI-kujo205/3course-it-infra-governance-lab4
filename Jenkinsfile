pipeline {
    agent any
    tools {
        nodejs 'node'  
    }
    stages {
        stage('Checkout Code') {
            steps {
                git url: 'https://github.com/KPI-kujo205/3course-it-infra-governance-lab4',
            }
        }
        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }
        stage('Run Tests') {
            steps {
                sh 'npm test'
            }
        }
    }
}

