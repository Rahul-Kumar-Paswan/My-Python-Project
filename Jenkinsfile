pipeline {
  agent any
  
  stages{
    stage('version') {
      steps {
        echo "Hello Dear"
      }
    }
    stage('checking') {
      steps {
        echo " hello dear welcome to  my world !!!!"
      }
    }
    
    stage('build') {
      steps {
        echo "hello"
        sh 'docker build -t my-python-project:1.2 .'
        sh 'docker tag my-python-project:1.2 rahulkumarpaswan/my-python-project:1.2'
        sh 'docker push rahulkumarpaswan/my-python-project:1.2'
        sh 'docker run -it -p 3000:3000 rahulkumarpaswan/my-python-project:1.2'
      }
    }
  }
}
