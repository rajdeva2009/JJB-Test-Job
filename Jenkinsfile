#! groovy

node('') {
  sh "echo GitHub BranhName ${env.BRANCH_NAME}"
  def WORKSPACE = "/etc/jenkins_jobs"
  
  stage('checkout') {
    sh "cd ${WORKSPACE}"
    git branch: 'master',credentialsId: '78f2dae7-0d97-446d-b047-aae8324b7c43', url: 'https://github.com/rajdeva2009/JJB-Test-Job.git'
  }
  
  stage('data') {
    sh "cd ${WORKSPACE};ls -ltr"
  }
}
