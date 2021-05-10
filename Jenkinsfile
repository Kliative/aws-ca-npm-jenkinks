pipeline {
    agent any

    tools {nodejs "node"}
    stages {
        stage('Stage 1') {
            steps {
                echo '11Hello s git push --set-upstream origin 3 git push --set-upstream origin 3dfwaaasaaoeeerld!asdas 2'
            }
        }
        stage('Stage 2 Npm') {
            steps {
                echo 'NPM'
                
            }
        }
        stage('Deploy') {
            when {
                expression {
                    currentBuild.result == null || currentBuild.result == 'SUCCESS'
                }
            }
            steps {
                    sh 'npm publish'
                    echo 'I thinksskjlkjl this works'
            }
        }
    }
}
