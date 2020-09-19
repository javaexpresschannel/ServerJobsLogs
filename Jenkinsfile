pipeline {
    agent any 
    stages {
        stage('Copy Files') { 
            steps {
                sh "sudo cp -r /home/javaexpress/serverlogs/* . "
            }
        }
        
        stage('Archving') { 
            steps {
                 archiveArtifacts '*.log'
            }
        }
    }
}
