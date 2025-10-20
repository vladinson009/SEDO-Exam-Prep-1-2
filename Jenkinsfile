pipeline {
    agent any

    stages {
        stage('Restore NuGet packages') {
            steps {
                sh "dotnet restore"
            }
        }

        stage('Run the building prccess') {
            steps {
                sh "dotnet build"
            }
        }

        stage('Run Tests') {
            steps {
                sh "dotnet test"
            }
        }
    }
}