// Using git without checkout
pipeline {
  agent any
  
    parameters {
      
        gitParameter branchFilter: 'origin/(.*)', defaultValue: "${env.BRANCH_NAME}", name: 'BRANCH', type: 'PT_BRANCH'
    }
  
  stages {
    stage('Example') {
      steps {
                git branch: "${params.BRANCH}", credentialsId: 'dockerhub', url: 'https://github.com/alisial45/dummy_pipeline.git', tool: 'Default'
            }
      
    }
  }
}
