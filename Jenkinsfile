node('centos') {
    if(env.BRANCH_NAME == "develop") {      
    stage('SCM') {
    checkout scm
    }
    stage('List files') {
    sh "ls -ltr"
    }
    }
  else if(env.BRANCH_NAME == "release") {
    stage('Deploy the code') {
        echo " Deplpy into Pre Prod Server"
    }
  }
  else if(env.BRANCH_NAME == "master") {
      stage ('Deploy code itto PROD') {
        echo " Deploy into PROD Server"
      }
  }
}
