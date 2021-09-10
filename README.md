# Jenkinsfile-based-pipeline-Jenkins

Steps to run a pipeline in Jenkins through Jenkinsfile in Github repository

```

1. Create a Maven project and upload it to a git repository.

2. Create a Jenkinsfile and upload it to the same repository.
pipeline {	 
	agent any	 
    	stages {     	 
    	stage("Compile") {          	 
            	steps {               	 
                	sh "mvn compile"          	 
            	}     	 
        	}     	 
    	stage("Unit test") {          	 
        	steps {               	 
                	sh "mvn test"          	 
            	}     	 
        	}	 
    	}
}

3. Create a pipeline item in Jenkins and select pipeline as Pipeline script from SCM, add the Git repository URL.

4. Build the pipeline job and view the console output.

```
