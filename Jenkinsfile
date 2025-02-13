pipeline {
    agent any

    stages {
		stage('Restore NuGet Packages') {
            steps {
				bat 'dotnet restore'
            }
        }
		stage('Build Project') {
            steps {
				bat 'dotnet build'
            }
        }
		stage('Run Dotnet Test') {
            steps {
				bat 'dotnet test'
            }
        }
    }
}