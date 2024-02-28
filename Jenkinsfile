pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                script {
                    def branchName = sh(returnStdout: true, script: 'git rev-parse --abbrev-ref HEAD').trim()
                    echo "Branch Name: ${branchName}"
                }
            }
        }
    }
}
