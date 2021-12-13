pipeline {
    agent any 
    stages {
        stage ('clean & Compile stage') { 
            steps {
             sh 'mvn clean'
            }
        }
        stage ('validate Stage') { 
            steps {
             sh 'mvn validate'
            }
        }
        stage ('Test Stage') { 
            steps {
             sh 'mvn test'
            }
        }
        stage ('Build Stage') { 
            steps {
             sh 'mvn package'
        }
    }
}
}
