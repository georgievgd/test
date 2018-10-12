def label = "python_agent"
//def label = "test"

node(label) {

    stage('Source') {
        checkout scm
    }

    stage('Build') {
        sh "sleep 1s;"
        sh "whoami;pwd;ls -al;"
    }
    
    stage('Test') {
        sh "sleep 1s;"
        try {
            sh "python --version"
        }
        catch (exc) {
            echo 'Something failed, I should sound the klaxons!'
        }
    }
    
    stage('Documentation') {
        sh "sleep 1s;"
    }

    stage('Deploy') {
        sh "sleep 1s;"
    }
}