pipeline {
    agent any
    stages {
        stage('Build'){
            steps{
                bat 'npm install'
            }
        }
        stage('Test Command'){
            steps{
                powershell '''Write-Output "Hello World!"
                $date = Get-Date
                Write-Output "Current Date and time : $date"
                '''
            }
        }
        stage('Test Command1'){
            steps{
                 powershell '''./myscript.ps1'''                               
            }
        }
    }
}