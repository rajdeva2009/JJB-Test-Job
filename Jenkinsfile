#! groovy

node('') {
  sh "echo GitHub BranhName ${env.BRANCH_NAME}"
  def WORKSPACE = "/etc/jenkins_jobs"
  
  stage('checkout') {
    sh "cd ${WORKSPACE}"
    git branch: 'master',credentialsId: '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', url: 'https://github.com/rajdeva2009/JJB-Test-Job.git'
  }
  
  stage('data') {
    sh "cd ${WORKSPACE};ls -ltr"
  }
}
