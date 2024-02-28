// Using git without checkout
pipeline {
  agent any
      parameters {
      gitParameter branchFilter: 'origin/(.*)', defaultValue: "${BRANCH_NAME}", name: 'BRANCH', type: 'PT_BRANCH'
    
    }
 
    stage('Example') {
      steps {
        git branch: "${params.BRANCH}", credentialsId: 'forwebhook', url: 'https://github.com/alisial45/dummy_pipeline.git', tool: 'Default'
      }
    }
  }
}
