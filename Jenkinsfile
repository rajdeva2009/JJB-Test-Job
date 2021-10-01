#! groovy

node('') {
  echo "GitHub BranhName ${env.BRANCH_NAME}"
  
  stage('checkout') {
    git branch: 'master',url: '   '
  }
  
  stage('data') {
    sh "echo ${WORKSPACE}"
  }
}
