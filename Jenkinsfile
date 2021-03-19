pipeline {
    agent any

    tools {
        maven 'default'
    }

    stages {
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
    
    post {
        always {
            
            junit 'target/surefire-reports/**/*.xml'
        }
    }
}
