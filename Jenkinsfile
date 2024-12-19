pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=gurutest_gurutest -Dsonar.organization=gurutest -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=5b16f93d8764f9bbc9ea124363132fb333ca4936'
			}
        } 
  }
}
