pipeline{
    agent any
    
    tools{
        gradle "gradle"
    }
    stages{
        stage("clone code"){
            steps{
                git branch: "master", url: "https://github.com/hodhanhassan99/java-todo.git"
            }
        }
        stage("build code"){
            steps{
                sh "gradle build"
            }
        }
        stage("test code"){
            steps{
                echo "gradle test"
            }
        }
        stage("deploy code"){
            steps{
                echo "deploying.."
            }
        }
    }
}