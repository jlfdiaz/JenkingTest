node  {
    checkout scm
    stage('Build') {
            withMaven (
            maven:'Maven Test'
            ) {
        sh 'mvn compile'
        }
    }
    stage('Test') { 
            withMaven (
            maven:'Maven Test'
            ) {
        sh 'mvn test'
        }
    }
    stage('Deploy') { 
            withMaven (
            maven:'Maven Test'
            ) {
        sh 'mvn package'
        }
        DeleteDir();
    }
}
