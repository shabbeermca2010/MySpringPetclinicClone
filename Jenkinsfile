pipeline {
    agent any
    stages {
        stage('vcs') {
            steps {
                git branch: "main", url: 'https://github.com/shabbeermca2010/MySpringPetclinicClone/'
            }
            
        }
        stage('Build the Code') {
            steps {
               bat 'mvn clean install'
            }
        }
        
    }

}
