pipeline 
{
   agent any

   stages
	{
	stage('checkout')
		{
   		 steps{
        		script{
           			 checkout scm
       			       }
    			}
		}
      stage('Build') 
		{
         	steps 
			{
           			 // Get some code from a GitHub repository
           			 git 'https://github.com/narendra1997/assignment1.git'

           			 // Run Maven on a Unix agent.
           			 sh "mvn clean install -DskipTests"
				

          
         		}
     		 }
	}}
