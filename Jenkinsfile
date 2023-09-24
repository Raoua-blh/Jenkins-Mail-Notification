pipeline {
    agent any
    
    stages {
        stage('Display and Email README.md Content') {
            steps {
                script {
                    // Read the contents of README.md using 'cat' command
                    def readmeContents = sh(script: 'cat README.md', returnStdout: true).trim()
                    
                    // Print the contents to the console
                    echo "Contents of README.md:\n${readmeContents}"
                    
                    // Send an email with the contents of README.md
                    emailext (
                        subject: 'Contents of README.md',
                        body: readmeContents,
                        to: 'your-email@example.com'
                    )
                }
            }
        }
    }
}
