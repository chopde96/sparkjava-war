pipeline {                                    // 1  // Defines the start of the Jenkins pipeline block
    agent any                                 // Specifies the pipeline can run on any available agent
    environment {                             // 2  // Defines environment variables for the pipeline
        PATH = "/opt/maven/bin:$PATH"         // Adds Maven's path to the system's PATH variable
    }                                         // 2  // Ends the environment block
    stages {                                  // 3  // Defines the stages block where multiple stages are declared
        stage('build') {                      // 6  // Creates a stage named 'build'
            steps {                           // 7  // Defines the steps that will be executed in this stage
                sh 'mvn clean install'        // Runs the Maven clean install command to build the project
            }                                 // 7  // Ends the steps block for 'build' stage
        }                                     // 6  // Ends the 'build' stage
    }                                         // 3  // Ends the stages block
}                                             // 1  // Ends the pipeline block
