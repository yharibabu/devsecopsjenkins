pipeline {
  agent any
  tools { 
        maven 'Maven_3.5.2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=azuredevsecopsprojkey -Dsonar.organization=azuredevsevopsorg -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=363be6d11281420f0cc3ba072d8b88039f970472'
			}
        } 
  }
}
