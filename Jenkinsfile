pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Running build automation'
                sh 'cd /opt/gradle/gradle-5.0/bin'
                sh 'gradle build'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}
