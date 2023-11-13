// do the import
import io.wcm.devops.jenkins.pipeline.utils.logging.LogLevel
import io.wcm.devops.jenkins.pipeline.utils.logging.Logger
import static io.wcm.devops.jenkins.pipeline.utils.ConfigConstants.*

// initialize the logger 
Logger.init(this, [ (LOGLEVEL) : LogLevel.WARN] )
Logger log = new Logger(this)

pipeline {
    agent any
    stages {
	    stage("First") {
            steps {
                echo "Something"
                // greet "Traveller"
            }
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