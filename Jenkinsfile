#!/usr/bin/env groovy
//dockerNode(credentialsId: 'docker-swarm', dockerHost: 'tcp://dcorley-swarm-mgr01.usc.edu:2376', image: 'hello-world', remoteFs: '') {
//   echo Hello World
//}
node {
    checkout scm

    docker.withServer('tcp://dcorley-swarm-mgr01.usc.edu:2376', 'docker-swarm') {
        docker.image('mysql:5').withRun('-p 3306:3306') {
            /* do things */
        }
    }
}/*pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                    checkout scm */
                    /* .. snip .. */
/*                    echo 'Building..'
                echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
                echo "Running ${env}"
                sh "env"
                sh "${env}"
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
*/