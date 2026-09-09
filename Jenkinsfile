pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Task: Compile and package the application code.'
                echo 'Tool: Apache Maven'
            }
        }

        stage('Unit and Integration Tests') {
            steps {
                echo 'Task: Run unit tests and verify that application components work together.'
                echo 'Tools: JUnit and Postman'
            }
        }

        stage('Code Analysis') {
            steps {
                echo 'Task: Analyse code quality and check compliance with coding standards.'
                echo 'Tool: SonarQube'
            }
        }

        stage('Security Scan') {
            steps {
                echo 'Task: Scan the application and its dependencies for security vulnerabilities.'
                echo 'Tool: OWASP Dependency-Check'
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo 'Task: Deploy the application to a staging environment.'
                echo 'Tool: AWS CLI with an AWS EC2 staging instance'
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo 'Task: Test the application in the production-like staging environment.'
                echo 'Tool: Postman with Newman'
            }
        }

        stage('Deploy to Production') {
            steps {
                echo 'Task: Deploy the tested application to the production server.'
                echo 'Tool: AWS CLI with an AWS EC2 production instance'
            }
        }
    }
}
