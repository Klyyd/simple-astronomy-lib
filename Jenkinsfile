pipeline {
  agent any
  
  stages {
    stage ('Build') {
      steps {
        echo 'Building ...'
        'mvn -B -DskipTests clean package'
      }
      post {
          success {
            junit '*/target/surefire-reports/TEST-.xml'
            archiveArtifacts 'target/*.jar'
        }
      }
    }
    
    stage ('Test') {
      steps { 
        echo 'Testting ...'
        sh 'mvn test'
      }
      post {
        always {
          junit 'target/surefire-reports/*.xml'
        }
      }
    }
    
    stage ('Generate') {
      steps {
        echo 'Generating ...'
      }
    }
    
    stage ('Deploy') {
      steps {
        echo 'Deploying ...'
      }
    }    
  }
}
