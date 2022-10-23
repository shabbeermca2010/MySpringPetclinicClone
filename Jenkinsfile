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
                                        cd C://ProgramData/Jenkins/.jenkins/jobs/sample multibranch/branches/dev/workspace/target
              					        junit allowEmptyResults: true, testResults: '**/test-results/*.xml'
                     					archiveArtifacts 'target/*.jar'
            
                				}
        
                
            				}
        }
    }
