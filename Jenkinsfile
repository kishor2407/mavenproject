pipeline
{
    agent any
    stages {
		stage('SCM-Checkout')
		{
			steps{ git 'https://github.com/kishor2407/mavenproject.git'} 
		}
	    
	    	stage('Execute-UnitTest')
                {
			steps{ withMaven(globalMavenSettingsConfig: '', jdk: 'JAVA_HOME', maven: 'MAVEN_HOME', mavenSettingsConfig: '', traceability: true) {
				sh 'mvn test'}}
		}
		    
	}
}
