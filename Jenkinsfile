pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'mvn verify'
            }
        }
    }
    post {
        always {
            junit 'build/reports/**/*.xml'
        }
    }
}
