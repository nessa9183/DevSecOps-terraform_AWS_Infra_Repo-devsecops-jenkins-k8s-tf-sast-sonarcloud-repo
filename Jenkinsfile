pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=nessagbuggywebapp -Dsonar.organization=nessabuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=42492d5b384d667242a8677842b49d83d1140f3e'
			}
        } 
  }
}
