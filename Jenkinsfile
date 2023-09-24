pipeline {
    agent any
    
    stages {
        stage('Display README.txt Content') {
            steps {
                script {
                    // Read the contents of README.txt using 'cat' command
                    def readmeContents = sh(script: 'cat README.txt', returnStdout: true).trim()
                    
                    // Print the contents to the console
                    echo "Contents of README.txt:\n${readmeContents}"
                }
            }
        }
    }
}
