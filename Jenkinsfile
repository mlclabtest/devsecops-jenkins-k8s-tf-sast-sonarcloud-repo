pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=lab8kswebapp -Dsonar.organization=lab8kswebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=07bb9b62e6ca081c7ab548116fcfe9d43aad2046'
			}
        } 
  }
}
