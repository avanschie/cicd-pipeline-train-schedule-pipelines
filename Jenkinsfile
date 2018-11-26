pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Running build automation'
                sh './gradlew build --now-daemon'
                archiveArtifact artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}
