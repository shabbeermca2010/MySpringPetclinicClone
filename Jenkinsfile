pipeline 

   {
    agent any

    triggers 
					{
        				cron('* 18 * * 1-5')
             		}
    stages {
        		stage('vcs') {  
            				steps {
                						git branch: "qa", url: 'https://github.com/GitPracticeRepo/MySpringPetclinicClone.git'
            						}
            
        						}
         stage ('Artifactory configuration') {
             				steps{             
              							junit '**/target/surefire-reports/TEST-*.xml'
                     					archiveArtifacts 'target/*.jar'
            
                				}
        
                
            										}
        }
    }
