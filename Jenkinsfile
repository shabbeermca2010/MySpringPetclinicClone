pipeline 

   {
    agent any

    triggers 
					{
        				cron('* 18 * * 1-5')
             		}
    stages {
        		
        						}
         stage ('Artifactory configuration') {
             				steps{             
              					        junit '**/target/surefire-reports/TEST-*.xml'
                     					archiveArtifacts 'target/*.jar'
            
                				}
        
                
            										}
        }
    }
