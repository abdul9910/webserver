pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps{

                withMaven(maven : 'Movan'){
                    sh 'mvn clean compile'

                }
                    
            }
        }
   stages {
        stage ('Testing Stage') {

            steps{

                withMaven(maven : 'Movan'){
                    sh 'mvn test'

                }
                    
            }
        }
           stages {
        stage ('Deploy Stage') {

            steps{

                withMaven(maven : 'Movan'){
                    sh 'mvn clean deploy'

                }
                    
            }
        }
    }    
