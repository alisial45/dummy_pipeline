pipeline {
    agent any
 parameters {
        gitParameter   defaultValue: 'main', name: 'BRANCH', type: 'BRANCH'
    }     
    stages {
        stage('Checkout') {
            steps {
                script {
                         git url: 'https://github.com/alisial45/dummy_pipeline.git', 
                         credentialsId: 'dockerhub', 
                         branch: "${params.BRANCH}"
                }
            }
        }
        // Other stages of your pipeline
    }
}
