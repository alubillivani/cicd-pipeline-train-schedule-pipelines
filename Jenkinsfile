pipeline {
    agent any 
    stages {
	 stage('Pull Code'){
		steps{
			git credentialsId: 'GitCred', url: 'https://github.com/alubillivani/cicd-pipeline-train-schedule-pipelines'
		    }		    
	 }	    
        stage('Build') { 
            steps {
		echo 'Build stage'
                sh './gradlew build'
		archiveArtifacts 'dist/trainSchedule.zip'
            }
        }
        
    }
}
