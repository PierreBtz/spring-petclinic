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
            junit 'target/surefire-reports/**/*.xml'
        }
    }
}
