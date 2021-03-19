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
                sh '''#!/bin/bash
                      df
                '''
            }
        }
    }
}
