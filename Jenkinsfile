pipeline {
    agent any
    stages {      
         stage('Clone Repo') {
            steps {
                /* groovylint-disable-next-line LineLength */
                git([url: 'https://github.com/alisial45/dummy_pipeline.git', branch: "one-parameterized", credentialsId: 'forwebhook'])
            }
        }
        }
    }



