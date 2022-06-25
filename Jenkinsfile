
pipeline{
    agent any
    stages{
     
        stage("Build with maven"){
            steps{
                sh 'mvn clean package'
            }
        }
        stage("Save Artifacts"){
            steps{
              archiveArtifacts artifacts: '**/*.jar', followSymlinks: false
            }
            
        }
    }
}