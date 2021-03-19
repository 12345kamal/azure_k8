pipeline {
    agent any
    stages {
        stage('sample Stage') {
            steps {
                echo 'This pipeline is to intergrate azure k8 service'
            }
        }
        stage('NORMAL Stage') {
            steps {
                sh '''
                      az aks create --resource-group 1-23e1741a-playground-sandbox --name MyManagedCluster
                '''
            }
        }
        stage('NORMAL Stage') {
            steps {
                sh '''
                      kubectl get nodes -o wide
                '''
            }
        }
    }
}
