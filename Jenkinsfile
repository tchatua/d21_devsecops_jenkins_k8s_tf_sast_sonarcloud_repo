pipeline {
  agent any
  tools { 
        maven 'maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbrokenwebapp -Dsonar.organization=asgbrokenwebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=c4747beb4222a7a747b8e24dec8c85abf3327cce'
			}
        } 
  }
}

