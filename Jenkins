pipeline {
    agent none
    stages {
	    stage("First") {
            echo "Something"
            greet "Traveller"
        }
		stage ('Middle-1') {
            steps {
                // log.info 'Starting' 
                script { 
                    log.info 'Middle-1'
                    log.warning 'Nothing to do!'
                }
            }
        }
        stage("Middle-2") {
            //HelloWorld obj = new HelloWorld();
            //echo obj.sayHello("Hello World from Test")
        }
        stage("Last") {
            echo "We're done"
        }
    }
}