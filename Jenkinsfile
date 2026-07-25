pipeline {
    agent any
    environment{
        APP_NAME = "Test-APP"
        APP_VERSION = "1.0.0"
        APP_ENV = "dev"
    }
    
    stages{
        stage("Build"){
            steps{
                echo "Build Application.."
                echo "App name is ${APP_NAME}"
                echo "App Version is ${APP_VERSION}"
                echo "NEED to run in ${APP_ENV}"
            }
        }
        stage("Test"){
            steps{
                echo "Test Application"
                echo "App name is ${APP_NAME}"
                echo "App Version is ${APP_VERSION}"
                echo "NEED to run in ${APP_ENV}"
            }
        }
        stage("Deploy"){
            steps{
                echo "DEploy Application"
                echo "App name is ${APP_NAME}"
                echo "App Version is ${APP_VERSION}"
                echo "NEED to run in ${APP_ENV}"
            }
        }
    }
    post{
        success{
            echo "pipeline is successful"
        }
        failure{
            echo "Pipeline failed"
            
        }
        always{
            echo "This should run whether the pipeline fail or success"
        }
    }
}
