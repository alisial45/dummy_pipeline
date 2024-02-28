pipeline {
    agent any

    parameters {
        string(name: 'GIT_BRANCH', defaultValue: 'master', description: 'Name of the branch to build')
    }
    stages {
        stage('Hello') {
            steps {
                script {
                    def branchName = params.GIT_BRANCH
                  
                    echo "Building branch: ${branchName}"
                    // Add steps to build the specified branch
                }
            }
        }
    }
}







