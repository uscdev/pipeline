#!/usr/bin/env groovy
//dockerNode(credentialsId: 'docker-swarm', dockerHost: 'tcp://dcorley-swarm-mgr01.usc.edu:2376', image: 'hello-world', remoteFs: '') {
//   echo Hello World
//}
pipeline {
    agent any

    stages {
        node {
            checkout scm
            /* .. snip .. */
        }
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
