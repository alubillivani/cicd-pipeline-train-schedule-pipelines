pipeline {
    agent any 
    stages {	
	stage('PullCode') { 
            steps {
		git 'https://github.com/alubillivani/cicd-pipeline-train-schedule-pipelines'
            }
        }
        stage('Build') { 
            steps {
		echo 'Build stage'
                sh './gradlew build --no-daemon'
		archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
        
    }
}
