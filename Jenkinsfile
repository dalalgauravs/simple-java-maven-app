pipeline {
    agent {
        docker {
            image 'maven:3-alpine'
            args '-v C:\Users\dalalgau\.m2\pipeline-jenkins:/root/.m2'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn -B -DskipTests clean package'
            }
        }
    }
}