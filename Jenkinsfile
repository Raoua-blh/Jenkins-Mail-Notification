pipeline {
    agent any
    
    stages {
        stage('Read README.txt') {
            steps {
                // Read the contents of README.txt
                def readmeContents = readFile('README.txt')
                
                // Print the contents to the console (you can modify this as needed)
                echo "Contents of README.txt:\n${readmeContents}"
                
                // Send an email with the contents of README.txt
                emailext (
                    subject: 'New commit: Contents of README.txt',
                    body: readmeContents,
                    to: 'rawaa.blh@gmail.com'
                )
            }
        }
    }
}
