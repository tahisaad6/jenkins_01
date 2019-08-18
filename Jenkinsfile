pipeline {
    agent any
 environment {
 
    PATH = "C:\\Program Files\\Git\\usr\\bin;${env.PATH}"
    stages {
        stage ('Compile Stage') {

            steps {
               
                    sh 'mvn clean compile'
                
            }
        }

        stage ('Testing Stage') {

            steps {
               
                    sh 'mvn test'
                
            }
        }


        stage ('Deployment Stage') {
            steps {
               
                    sh 'mvn deploy'
                
            }
        }
    }
    
   }
}
