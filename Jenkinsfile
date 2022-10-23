pipeline 

   {
    agent any

    triggers 
					{
        				cron('* 18 * * 1-5')
             		}
    stages {
        		
        						
         stage ('Artifactory configuration') {
             				steps{             
              					        junit allowEmptyResults: true, testResults: '**/test-results/*.xml'
                     					archiveArtifacts 'target/*.jar'
            
                				}
        
                
            				}
        }
    }
