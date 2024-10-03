pipeline {
  agent any
  environment { 
    DOCKER_ID = "dstdockerhub"
    DOCKER_IMAGE = "datascientestapi"
    DOCKER_TAG = "v.${BUILD_ID}.0" 
  }
  stages {
    stage ('Building'){
      step {
        sh 'pip install -r requirements.txt 
      }
    }
    stage ('Testing'){
      step {
        sh 'python -m unitest
      }
    }
    stage ('Deploying'){}
  }
}
