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
                sh "node sum.test.js"
            }
        }
        stage('deploy') {
            steps{
                sh "node index.js"
            }
        }
    }
}