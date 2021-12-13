pipeline {
    agent any 
    stages {
        stage ('clean & Compile stage') { 
            steps {
                withMaven(maven : 'MAVAN_HOME') {
                   sh 'mvn clean compile'
                }
            }
        }
        stage('validate Stage') { 
            steps {
                withMaven(maven : 'MAVAN_HOME') {
                   sh 'mvn validate'
                }
            }
        }
        stage('Test Stage') { 
            steps {
                withMaven(maven : 'MAVAN_HOME') {
                   sh 'mvn test'
                }
            }
        }
        stage('Build Stage') { 
            steps {
                withMaven(maven : 'MAVAN_HOME') {
                   sh 'mvn package'
            }
        }
    }
}
}
