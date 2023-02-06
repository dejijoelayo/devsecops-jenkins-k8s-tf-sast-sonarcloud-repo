pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=dejijoelayo -Dsonar.organization=dejijoelayo -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=79c11ecfe8b84cc843d2059704fb142535589648'
			}
        } 
  }
}
