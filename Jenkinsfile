pipeline {
  agent { label 'electronix' }

  stages {
    stage ('Hello'){ steps { echo "Hello Jenkins" }  }
    stage ('Hello-second'){ steps { echo "Hello Jenkins Second" }  }
  } 
  post {
    success {
      echo "Pipline Pass"
      mail to : "annusingh12112003@gmail.com",
      subject : "SUCCESS"
      body : "email working"
    }
    failure{
      echo "Pipline Fail"
    }
  }
}


  
