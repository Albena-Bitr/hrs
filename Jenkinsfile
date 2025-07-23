pipeline{
    agent any
    stages{
        stage('Restore'){
            steps{
                bat 'dotnet build HouseRentingSystem.sln'
            }
        }
        stage('Build the app'){
            steps{
                bat 'dotnet build HouseRentingSystem.sln --configuration Release'
            }
        }
        stage('Run tests'){
            steps{
                bat 'dotnet test HouseRentingSystem.Tests/HouseRentingSystem.Tests.csproh'
            }
        }
    }
}
