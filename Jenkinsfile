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
                echo "this is dev deploy ${DEV_ENV}"            
                
            }
        }
        stage('Test') {
            steps {
                echo "{$TEST_ENV}"
            }
        }
        
        stage('Stage') {
            steps {
                echo "{$STAGE_ENV}"
            }
        }
        
        stage('Prod') {
            steps {
                echo "{$PROD_ENV}"
            }
        }
        
        
    }
}
