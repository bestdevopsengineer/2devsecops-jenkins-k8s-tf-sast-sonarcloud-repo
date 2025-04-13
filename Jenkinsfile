pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=2025-asgbuggywebapp -Dsonar.organization=2025-asgbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=99258b308746ac519c965c826664bb97905cd6e2'
			}
        } 
  }
}
