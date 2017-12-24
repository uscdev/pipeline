#!/usr/bin/env groovy
//dockerNode(credentialsId: 'docker-swarm', dockerHost: 'tcp://dcorley-swarm-mgr01.usc.edu:2376', image: 'hello-world', remoteFs: '') {
//   echo Hello World
//}
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                node any {
                    checkout scm
                    /* .. snip .. */
                }
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
