#!/usr/bin/env groovy
//dockerNode(credentialsId: 'docker-swarm', dockerHost: 'tcp://dcorley-swarm-mgr01.usc.edu:2376', image: 'hello-world', remoteFs: '') {
//   echo Hello World
//}
pipeline {
    agent any

    stages {
        stage('Build') {
            node {
                checkout scm
                /* .. snip .. */
            }
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
