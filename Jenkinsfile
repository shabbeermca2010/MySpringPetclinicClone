pipeline 
   {
    agent any

    triggers 
		{
        		cron('* 18 * * 1-5')
             	}
           post
            {
            always
            {
                // If Maven was able to run the tests, even if some of the test
                // failed, record the test results and archive the jar file.
                
                    junit '**/target/surefire-reports/TEST-*.xml'
                     archiveArtifacts 'target/*.jar'
                   
                }
            
            }
    
        }
    
