pipeline {
    agent any

    stages {
        stage('gitBigbillionsale') {
            steps {
                checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'manojthirumani-jenkins', url: 'https://github.com/manojthirumani/Bigbillionsale.git']]])
            }
        }
        stage('checkout') {
            steps {
            echo 'checkout project'    
                } }
                stage('build') {
            steps {
            echo 'buliding project'    
                } }
                stage('test') {
            steps {
            echo 'testing project'    
                } }
                stage('QA Deploy') {
            steps {
            echo 'QA Deploy project'    
                } }
                stage('prod deploy') {
            steps {
            echo 'prod deploy project'    
                } }
           }
}
