pipeline {
    agent any

    stages {
      
        stage('mail notif') {
            steps {
                emailext body: readFile('README.txt'), subject: 'New Commit', to: 'bhjrou5@gmail.com'
            }
        }
    }
}
