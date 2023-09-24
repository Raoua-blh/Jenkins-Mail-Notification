pipeline {
    agent any
    
    stages {
        stage('email Notif ') {
            steps {
                script {
                    def readmeContents = sh(script: 'cat README.md', returnStdout: true).trim()

                    echo "Contents of README.md:\n${readmeContents}"
                    
          
                    emailext (
                        subject: 'from Rawaa Ben Hadj Amor Mail Notif Jenkins TP',
                        body: readmeContents,
                        to: 'rawaa.blh@gmail.com'
                    )
                }
            }
        }
    }
}
