pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=testnakibadevsecops_buggytest -Dsonar.organization=testnakibadevsecops -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=7f87ba68e78df43450e7d11dabb0f4265b28d2d6'
			}
        } 
  }
}
