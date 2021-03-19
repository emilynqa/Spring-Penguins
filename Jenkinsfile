pipeline {
    agent any

    tools {
        maven 'default'
    }

    stages {
        stage('Build') {
            steps {
                sh 'mvn -B package'
            }
        }
    }
}
