pipeline {
    agent any

    tools {nodejs "node"}
    stages {
        stage('Stage 1') {
            steps {
                echo 'Hello waaasaaoeeerld!asdas 2'
            }
        }
        stage('Stage 2 Npm') {
            steps {
                echo 'NPM'
                sh 'npm publish'
            }
        }
        stage('Deploy') {
            when {
                expression {
                    currentBuild.result == null || currentBuild.result == 'SUCCESS'
                }
            }
            steps {
                    echo 'I thinkss this works'
            }
        }
    }
}
