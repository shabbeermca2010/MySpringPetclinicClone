pipeline {
    agent any
    triggers {
        pollSCM('* * * * *')
    }
    stages {
        stage('vcs') {
            steps {
                git branch: "dev", url: 'https://github.com/GitPracticeRepo/MySpringPetclinicClone.git'
            }
            
        }
        stage('Build the Code') {
            steps {
               
                    bat 'mvn clean package'
                }
            }
        }
        
    }
