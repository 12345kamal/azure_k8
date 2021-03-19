pipeline {
    agent any
    stages {
        stage('sample Stage') {
            steps {
                echo 'This pipeline is to intergrate azure k8 service'
            }
        }
        stage('create AKS') {
            steps {
                sh '''#!/bin/bash
                       /usr/local/bin/az aks create --resource-group 1-23e1741a-playground-sandbox --name MyManagedCluster
                '''
            }
        }
        stage('check cluster') {
            steps {
                sh '''#!/bin/bash
                       /usr/local/bin/kubectl get nodes -o wide
                '''
            }
        }
    }
}
