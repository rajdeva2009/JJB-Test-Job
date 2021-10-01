#! groovy

node('') {
  stage('checkout') {
    git branch: 'master',credentialsId: '78f2dae7-0d97-446d-b047-aae8324b7c43', url: 'https://github.com/rajdeva2009/JJB-Test-Job.git'
  }
  
  stage('data') {
    sh "cp -R jobs /etc/jenkins_jobs"
    sh "cd /etc/jenkins_jobs"
    sh "jenkins-jobs update jobs"
  }
}
