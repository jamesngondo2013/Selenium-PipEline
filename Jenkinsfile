pipeline {

    agent any
    tools {
        maven 'MAVEN_HOME' 
    }
    stages {
        stage('Compile Stage') {
            steps {
                bat "mvn clean compile" 
        }
    }

         stage('Testing Stage') {
             steps {
                bat "mvn test verify"
        }
    }

          stage('Deployment Stage') {
              steps {
                bat "mvn deploy"
        }
    }

  }

}
