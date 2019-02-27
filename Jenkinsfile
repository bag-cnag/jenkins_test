pipeline {
    agent {
        label 'rdjenkins'
    }
/*    environment {
        AWS_ACCESS_KEY_ID     = credentials('dpiscia connection')
        
        
    }*/
    stages {

        stage('Example stage 2') {
    steps {
    wrap([$class: 'BuildUser']) {
      echo "${BUILD_USER}"
      echo "${BUILD_USER_ID}"
      echo "${BUILD_USER_EMAIL}"
    }
        }
    }
}


}
