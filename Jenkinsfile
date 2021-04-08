pipeline {
    agent any
    stages {
        stages {

        stage('SCM') {
            steps {
                checkout([$class: 'GitSCM', branches: [[name: '*/Develop']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/shab-a88/teaapp.git']]])
            }
        }

        stage("build") {
            steps{
                sh 'dotnet build "$WORKSPACE"'
            }
            
        }
    }
}