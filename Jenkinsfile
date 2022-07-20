pipeline {
    agent any

    stages {
        stage('Package') {
            steps {
                sh './mvnw package'
            }
        }
        stage('Save jar') {
            steps {
                archiveArtifacts artifacts: 'target/cc-spring-test-0.0.1-SNAPSHOT.jar', followSymlinks: false
            }
        }
    }
}
