pipeline {                              // start our pipeline -FIRE!
    agent any
    stages {
        stage('Verification Step') {          // stage 1 - "verification"
            steps {                           // first step produces NULL or NOT NULL
                sh '''my_var=$GIT_BRANCH        
                if [ -z "$my_var" ]
                then
                      echo "\\$my_var is NULL and the pipeline is working fine"
                else
                      echo "\\$my_var is NOT NULL but still the pipeline is working fine :)"
                fi'''
            }                           // end of step
        }                               // end of stage 1 - 'Verification Step'
    }                                   // end of stages
}                                       // end of pipeline
