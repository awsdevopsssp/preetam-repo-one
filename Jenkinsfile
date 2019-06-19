node {
    stage('SCM') {
    checkout scm
    }
    stage('List files') {
    sh "ls -ltr"
    }
    stage('Run Script') {
    sh "sh ssp.sh"
    }
}
