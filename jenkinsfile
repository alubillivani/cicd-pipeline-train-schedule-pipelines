pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
		            echo 'Build stage'
                sh './gradlew build'
		            archiveArtifacts 'dist/trainSchedule.zip'
            }
        }
        
    }
}
