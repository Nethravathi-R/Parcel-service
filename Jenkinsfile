pipeline {
    agent {
        label 'java'
    }

        stages {
        stage('checkout') {
            steps {
        sh 'rm -rf Parcel-service'
        sh 'git clone https://github.com/Nethravathi-R/Parcel-service.git'
      }
        }

        stage('build') {
            steps {
                script {
                    sh 'mvn --version'
                    sh 'mvn clean install'
                }
            }
        }

}
}
