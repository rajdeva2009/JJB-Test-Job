#! groovy

node('') {
  sh "echo GitHub BranhName ${env.BRANCH_NAME}"
  def WORKSPACE = "/etc/jenkins_jobs"
  
  stage('checkout') {
    sh "cd ${WORKSPACE}"
    git branch: 'master',credentialsId: 'Github_token', url: 'https://github.com/rajdeva2009/JJB-Test-Job.git'
  }
  
  stage('data') {
    sh "cd ${WORKSPACE};ls -ltr"
  }
}
