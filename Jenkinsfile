pipeline {
    agent any
    parameters {
        gitParameter(
            branchFilter: 'origin/(.*)',
            defaultValue: env.BRANCH_NAME, // Use BRANCH_NAME environment variable as default value
            name: 'BRANCH',
            type: 'PT_BRANCH'
        )
    }
    
    stages {
        stage('Example') {
            steps {
                script {
                    echo "Selected branch: ${params.BRANCH}"
                    // Use the branch name for further operations in the pipeline
                }
            }
        }
    }
}



