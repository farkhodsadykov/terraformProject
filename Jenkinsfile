// Authon Farkhod Sadykov
node {

  stage('Pull from githup') {
    git 'https://github.com/farrukh90/TerraformProject.git'
  }

  stage('Terrafrom init') {
    sh 'cd ${workspace}'
    sh 'terrafom init'
  }

  stage('Terrafrom plan') {
    sh 'terrafom plan -var region="${REGION}" -var appname="${APPNAME}" -var Environment="${ENV}"   -out=newplan -input=flase'
  }

}
