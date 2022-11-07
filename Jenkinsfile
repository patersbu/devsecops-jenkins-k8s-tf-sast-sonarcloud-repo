pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=patersbu-buggy-webapp -Dsonar.organization=patersbu-buggy-webapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=726273e66f4ea24ab95190c23660a1fef7dc3822'
			}
        } 
  }
}
