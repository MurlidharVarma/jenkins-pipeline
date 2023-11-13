// do the import
library identifier: 'jenkins-shared-library@main', retriever: modernSCM(
  [$class: 'GitSCMSource',
   remote: 'https://github.com/MurlidharVarma/jenkins-shared-library.git'])

pipeline {
    agent any
    stages {
	    stage("First") {
            steps {
                echo "Something"
                greet "Traveller"
            }
        }
		stage ('Middle-1') {
            steps {
                // log.info 'Starting' 
                script { 
                    echo 'Middle-1'
                    echo 'Nothing to do!'
                }
            }
        }
        // stage("Middle-2") {
        //     HelloWorld obj = new HelloWorld();
        //     echo obj.sayHello("Hello World from Test")
        // }
        stage("Last") {
            steps {
                echo "We're done"
            }
        }
    }
}