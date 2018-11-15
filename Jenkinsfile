node  {
    checkout scm
    stage('Build') {
            withMaven (
            maven:'Maven test'
            )
        sh 'mvn compile'
        }
    stage('Test') { 
            withMaven (
            maven:'Maven test'
            )
        sh 'mvn test'
        }
    stage('Deploy') { 
            withMaven (
            maven:'Maven test'
            )
        sh 'mvn package'
        }
}
