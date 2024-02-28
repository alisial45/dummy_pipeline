// Using git without checkout
pipeline {
  agent any
      parameters {
      gitParameter branchFilter: 'origin/(.*)', defaultValue: 'Branch-one', name: 'BRANCH', type: 'PT_BRANCH'
    
    }

  
    stage('Example') {
      steps {
        git branch: 'Branch-one', credentialsId: 'forwebhook', url: 'https://github.com/alisial45/dummy_pipeline.git', tool: 'Default'
      }
    }
  }
}
