pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebappjou -Dsonar.organization=asgbuggywebappjou -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=3e3384d1123496aba65a27ba10b9208212565c61'
			}
        } 
  }
}
