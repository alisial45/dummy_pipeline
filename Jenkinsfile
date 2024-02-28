pipeline {
    agent any
    
    parameters {
        gitParameter branchFilter: 'origin/(.*)', defaultValue: "${env.BRANCH_NAME}", name: 'BRANCH', type: 'PT_BRANCH'
    }  
    
    stages {

        stage('Debug') {
            steps {
                sh 'echo BRANCH_NAME: $BRANCH_NAME'
            }
        }
        
        stage('Example') {
            steps {
                git branch: "${params.BRANCH}", credentialsId: 'dockerhub', url: 'https://github.com/alisial45/dummy_pipeline.git', tool: 'Default'
            }
        }
    }
}


