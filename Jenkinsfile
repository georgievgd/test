def label = "python_agent"
//def label = "test"

node(label) {

    //logstashSend failBuild: true, maxLines: 1000
    logstash
    
    stage('Source') {
        checkout scm
    }

    stage('Build') {
        sh "sleep 1s;"
        sh "whoami;pwd;ls -al;"
    }

    stage('Check Styles') {
        sh "sleep 1s;"
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