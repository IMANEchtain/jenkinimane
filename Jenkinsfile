pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    // Change to the project directory
                    dir('C:/Users/ichtaini/AppData/Roaming/npm/proj') {
                        // Run the npm run start command
                        sh'cd C:\\Users\\ichtaini\\AppData\\Roaming\\npm\\proj && npm run start'
                        
                        // Capture the localhost URL
                        def localhostUrl = readFile('C:/Users/ichtaini/AppData/Roaming/npm/proj/localhost-url.txt')
                        echo "Localhost URL: $localhostUrl"
                    }
                }
            }
        }
    }
}
