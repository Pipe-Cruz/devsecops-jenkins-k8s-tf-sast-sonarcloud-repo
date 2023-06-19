pipeline {
  agent any
  tools { 
        maven 'Maven_3.5.2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=repotest -Dsonar.organization=Test -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=59e3f41fbbf11d200059d0f485439f56e8e5a386'
			}
        } 
  }
}
