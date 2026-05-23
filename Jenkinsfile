pipeline {
    agent any

    stages {
        stage('Cleanup Space') {
            steps {
                echo 'Cleaning up unused Docker resources...'
                // Xóa các dangling images và cache lỗi để giải phóng bộ nhớ trước khi build
                sh 'docker system prune -f'
            }
        }
        stage('Build') {
            steps {
                echo 'Building..'
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}