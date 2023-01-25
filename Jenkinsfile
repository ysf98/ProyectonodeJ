pipeline {
    agent any

    stages{
        stage('Linter') {
            steps{
                sh "node .eslintrc.json"
            }
        }
        stage('test') {
            steps{
                sh "npm install jest"
                sh "npm test"
            }
        }
        stage('deploy') {
            steps{
                sh "node index.js"
            }
        }
    }
}