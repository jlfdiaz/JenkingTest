node  {
    checkout scm
    stage('Build') {
            withMaven (
            maven:'Maven Build'
            )
        sh 'mvn compile'
        }
    stage('Test') { 
            withMaven (
            maven:'Maven Test'
            )
        sh 'mvn test'
        }
    stage('Deploy') { 
            withMaven (
            maven:'Maven Deploy'
            )
        sh 'mvn package'
        }
}
