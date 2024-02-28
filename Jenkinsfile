pipeline {
    agent any
 parameters {
        gitParameter   defaultValue: 'Branch-one', name: 'BRANCH', type: 'PT_BRANCH'
    } 
    stages {
        stage('Checkout') {
            steps {
                script {
                         git url: 'git@github.com:Productionmanager/productionmanager.git', 
                         credentialsId: 'produtionmanager', 
                         branch: 'Branch-one'
                }
            }
        }
        // Other stages of your pipeline
    }
}
