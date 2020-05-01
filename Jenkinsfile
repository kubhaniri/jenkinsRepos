pipeline {
    agent any
    stages{
        stage('Stage: Clean'){
            steps {
                withMaven(maven : 'Maven_3_6_3'){
                    sh 'mvn clean'
                }
            }
        }
        stage('Stage: Compile Stage'){
            steps {
                withMaven(maven : 'Maven_3_6_3'){
                    sh 'mvn compile'
                }
            }
        }
        stage('Stage: Test Stage'){
            steps {
                withMaven(maven : 'Maven_3_6_3'){
                    sh 'mvn test'
                }
            }
        }
        stage('Stage: deploy Stage'){
            steps {
                withMaven(maven : 'Maven_3_6_3'){
                    sh 'mvn deploy'
                }
            }
        }
    }
}