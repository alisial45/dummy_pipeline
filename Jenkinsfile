pipeline {
    agent any
     environment {
        DEFAULT_BRANCH = 'one-parameterized'
    }
      parameters {
        gitParameter branchFilter: 'origin/(.*)',  defaultValue: DEFAULT_BRANCH, name: 'BRANCH', type: 'PT_BRANCH'
    }
    stages {      
         stage('Clone Repo') {
             steps{
           echo env.GIT_BRANCH
             }
    
        }

        
    }
}






