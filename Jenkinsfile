pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo "Hello World"'
        sh '''
                    echo "Multiline shell steps work too"
                    ls -lah
                '''
        s3Upload(bucket: 'ucty-project', file: 'index.html')
      }
    }

  }
}