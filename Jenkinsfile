/* 需要Docker Pipeline插件 */
node('docker') {
    checkout scm
    stage('Build') {
        docker.image('python:latest').inside {
            sh 'python --version'
        }
    }
}
