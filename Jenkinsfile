#!/usr/bin/env groovy

pipeline {

    agent {
        docker {
            image 'node'
            args '-u root'
        }
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                sh 'npm install'
            }
        }
        // a new line for pushing a change
        // stage('Test') {
        //     steps {
        //         echo 'Testing...'
        //         sh 'npm test'
        //     }
        // }
    }
}
