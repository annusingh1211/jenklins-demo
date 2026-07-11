pipeline {
  agent { label 'electronix' }

  stages {
    stage ('Hello'){ steps { echo "Hello Jenkins" }  }
    stage ('Hello-second'){ steps { echo "Hello Jenkins Second" }  }
  } 
  post {
    success {
      echo "Pipline Pass"
    }
    failure{
      echo "Pipline Fail"
    }
  }
}


  
