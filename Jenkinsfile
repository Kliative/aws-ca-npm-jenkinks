pipeline {
    agent any
    stages {
        stage('Stage 1') {
            steps {
                echo 'Hello woeeerld!asdas 2'
            }
        }

        stage('Deploy') {
            when {
                expression {
                    currentBuild.result == null || currentBuild.result == 'SUCCESS'
                }
            }
            steps {
                    echo 'I think this works'
            }
        }
    }
}
