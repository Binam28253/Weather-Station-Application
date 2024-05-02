pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout source code from Git repository
                git 'https://github.com/your-username/weather-station.git'
            }
        }
        stage('Build') {
            steps {
                // Compile the main.c file
                sh 'gcc -o weather_station main.c' // Adjust compile command as needed
            }
        }
        stage('Test') {
            steps {
                // Run tests if available
                // Replace this with your test commands if you have any
                sh './weather_station' // Assuming you can execute your program for testing
            }
        }
    }
}
