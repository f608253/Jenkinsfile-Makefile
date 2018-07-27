// Declarative //
pipeline {
agent any
stages {
stage('Build') {
steps {
sh '''
cd /home/ec2-user/make
'''
sh 'make'
archiveArtifacts artifacts: '**/target/*.jar', fingerprint: true
}
}
}
}
