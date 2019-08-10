pipeline {
    agent any
    stages {
        stage('Upload to AWS') {
            steps {
                withAWS(region:'us-east-1', 'credentials': 'Jenkins') {
                    s3Upload(file:'index.html', bucket:'jenkinspipelines082019')
                }
            }
        }
    }
}
