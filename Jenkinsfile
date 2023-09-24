pipeline {
    agent any
    
    stages {
        stage('Display README.md Content') {
            steps {
                script {
                    // Read the contents of README.md using 'cat' command
                    def readmeContents = sh(script: 'cat README.md', returnStdout: true).trim()
                    
                    // Print the contents to the console
                    echo "Contents of README.md:\n${readmeContents}"
                }
            }
        }
    }
}
