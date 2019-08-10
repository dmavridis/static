pipeline {
    agent any
    stages {
        stage('Upload to AWS') {
            steps {
                withAWS(region:'us-east-1', credentials:'aws-static') {
                    sh 'echo "Hello World"'
//                    s3Upload(file:'index.html', bucket:'jenkinspipelines082019', )
                }
            }
        }
    }
}
