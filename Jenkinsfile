pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                script {
                    def branchName = sh(returnStdout: true, script: 'git rev-parse --abbrev-ref HEAD').trim()
                    if (branchName == 'HEAD') {
                        // We're in a detached HEAD state, let's retrieve the branch name differently
                        branchName = sh(returnStdout: true, script: 'git rev-parse --symbolic-full-name --abbrev-ref HEAD').trim()
                    }
                    echo "Branch Name: ${branchName}"
                }
            }
        }
    }
}
