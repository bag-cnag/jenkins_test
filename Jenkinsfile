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
        def safeBuildUser = "ujenkins"
            wrap([$class: 'BuildUser']) {
            try {
                safeBuildUser = BUILD_USER
            } catch (e) {
                    echo "User not in scope, probably triggered from another job"
                    }
            }
        echo "Builduser is: ${safeBuildUser}"
        
        }
    }
}


}
