node  {
    checkout scm
    stage('Build')  { sh 'mvn compile'}
    stage('Test') {sh 'mvn test'
                   junit '**/target/*.xml'
                  }
    stage('Deploy') { 
        withMaven { 
            maven 'Maven Test'
        }
        sh 'mvn package'
}
