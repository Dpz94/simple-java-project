pipeline {
    agent {
        docker { image 'maven:3-alpine' }
    }
    stages {
        stage ('test my code') {
               steps {
                   checkout scm 
                   sh 'mvn test'
               }
        }
        stage ('compile my code') {
            steps {
                sh 'mvn compile'
            }
        }
        stage ('package my code') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
               
