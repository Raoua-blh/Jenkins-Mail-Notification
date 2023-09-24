pipeline {
    agent any

    stages {
        stage('Display README.txt Content') {
            steps {
                script {
                    // Read the contents of README.txt
                    def readmeContents = readFile('README.txt')

                    // Print the contents to the console
                    echo "Contents of README.txt:\n${readmeContents}"
                }
            }
        }
    }
}
