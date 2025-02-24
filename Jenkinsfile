pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=vinayak-persistent -Dsonar.organization=vinayak-persistent -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=12416264909e93245f48ee1054d390dea5cf9394'
			}
        } 
  }
}
