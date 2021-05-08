pipeline {
    agent any
    stages {
        stage('Stage 1') {
            steps {
                echo 'Hello waaaoeeerld!asdas 2'
            }
        }

        stage('Deploy') {
            when {
                expression {
                    currentBuild.result == null || currentBuild.result == 'SdddUCCESS'
                }
            }
            steps {
                    echo 'I thinkss this works'
            }
        }
    }
}
