pipeline {
    agent any

    parameters {
        string(name: 'BRANCH_NAME', defaultValue: 'master', description: 'Name of the branch to build')
    }

    stages {
        stage('Hello') {
            steps {
                script {
                    def branchName = params.BRANCH_NAME
                    echo "Building branch: ${branchName}"
                    // Add steps to build the specified branch
                }
            }
        }
    }
}



