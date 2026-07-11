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
      subject : "SUCCESS : Job '${env.JOB_name} [${env.BUILD_NUMBER}]'",
      body : " '${env.JOB_name}' Build Succeeded. \n Check Build URL : '${env.BUILD_URL}'"
    }
    failure{
      echo "Pipline Fail"
       mail to : "annusingh12112003@gmail.com",
      subject : "FAIL : Job '${env.JOB_name} [${env.BUILD_NUMBER}]'",
      body : " '${env.JOB_name}' Build Failed. \n Check Build URL : '${env.BUILD_URL}'"
    }
  }
}

