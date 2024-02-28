// Using git without checkout
pipeline {
  agent any
      parameters {
      gitParameter branchFilter: 'origin/(.*)', defaultValue: 'Branch-one', name: 'BRANCH', type: 'PT_BRANCH'
    
    }
  
    stage('Example') {
     sh 'echo "hello"'
    }
  }
}

