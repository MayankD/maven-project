pipeline{
    agent any
    tools{
        maven 'Maven339'
        jdk 'Java8'
    }
    stages{
        stage ('init'){
            steps{
                echo "This is initializing stage"
            }
        }
        stage ('Build'){
            steps{
                echo "This is Build stage"
                sh label: '', script: 'clean package checkstyle:checkstyle'
            }
        }
        stage ('Deploy'){
            steps{
                echo "This is Deploy stage"
            }
        }
    }
}