pipeline {
    agent any
    
    parameters {
        gitParameter branchFilter: 'origin/(.*)', defaultValue: "${env.BRANCH_NAME}", name: 'BRANCH', type: 'PT_BRANCH'
    }
  
    stages {

         stage('Debug') {
            steps {
                script {
                    def gitTool = tool name: 'Default', type: 'hudson.plugins.git.GitTool'
                    echo "Git Tool: ${gitTool}"
                }
            }
        }

        
        stage('Example') {
            steps {
                git branch: "${params.BRANCH}", credentialsId: 'dockerhub', url: 'https://github.com/alisial45/dummy_pipeline.git', tool: '/usr/bin/git'
            }
        }
    }
}


