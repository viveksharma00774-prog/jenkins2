pipeline {
agent any
triggers { pollSCM('H/2 * * * *') }
stages {
stage('Build') { steps { sh 'sh app.sh' } }
stage('Test')  { steps { sh 'sh test.sh' } }
stage('Deploy') { steps { echo 'Deploying...' } }
}
}
