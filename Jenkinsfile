pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Running build automation on new project'
                sh 'chmod +x ./gradlew'
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}
