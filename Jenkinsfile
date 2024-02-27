// Using git without checkout
pipeline {
  agent any
  
    parameters {
        gitParameter branchFilter: 'origin/(.*)', defaultValue: "${env.BRANCH_NAME}", name: 'BRANCH', type: 'PT_BRANCH'
    }
  
  stages {
    stage('Example') {
      steps {
        sh 'echo hello'
        git branch: "${params.BRANCH}", url: 'https://github.com/alisial45/dummy_pipeline.git'
      }
    }
  }
}
