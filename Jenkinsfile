pipeline {
    agent any
    stages {

            stage("build") {
                steps {
                    sh 'dotnet build "$WORKSPACE/teaapp/teaapp.csproj"'
                }
                
            }
      
    }
}