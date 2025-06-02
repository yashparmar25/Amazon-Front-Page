pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                git 'https://github.com/yashparmar25/Amazon-Front-Page.git'
            }
        }

        stage('Archive Site Files') {
            steps {
                archiveArtifacts artifacts: '**/*.html, **/*.css, **/*.js, **/images/**', fingerprint: true
            }
        }

        stage('Deploy (Optional)') {
            steps {
                echo 'Deploy step – e.g., copy to web server or FTP (configure as needed)'
            }
        }
    }
}
