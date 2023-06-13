pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=bedtimebuggy -Dsonar.organization=bedtimebuggy -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=4cdcc51d4381d6024c742c468b23274a95b67fed'
			}
        } 
  }
}
