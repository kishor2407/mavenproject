pipeline
{
    agent any
    stages {
		stage('SCM-Checkout')
		{
			steps{ git 'https://github.com/kishor2407/mavenproject.git'} 
		}
		
	    	stage('Build')
                {
			steps{ sh 'echo Build_successful'}}
		}
}
