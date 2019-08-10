pipeline {
    agent any
    stages {
        stage('Upload to AWS') {
            steps {
                withAWS(region:'us-east-1', 'credentials': 'AKIA5QZZZ47OO6PXKRWA') {
                    s3Upload(file:'index.html', bucket:'jenkinspipelines082019')
                }
            }
        }
    }
}
