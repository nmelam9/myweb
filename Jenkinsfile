pipeline {
    agent { label 'dev'}
    environment {
        DEV_ENV = 'dev1'
        TEST_ENV = 'test'
        STAGE_ENV = 'stage'
        PROD_ENV = 'prod'
    }
        
    stages {
        stage('Dev') {
            steps {
                echo "this is dev deploy ${BUILD_ID}"            
                
            }
        }
        stage('Test') {
            steps {
                echo "{$BUILD_NUMBER}"
            }
        }
        
        stage('Stage') {
            steps {
                echo "{$JOB_NAME}"
            }
        }
        
        stage('Prod') {
            steps {
                echo "{$WORKSPACE}"
            }
        }
        
        
    }
}
