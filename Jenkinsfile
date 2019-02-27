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
        sh 'printenv'
    wrap([$class: 'BuildUser']) {
        
        if (env.BUILD_USER) {        
      echo "${BUILD_USER}"
        }
    }
        }
    }
}


}
