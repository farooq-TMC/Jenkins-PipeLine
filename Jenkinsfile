pipeline {
	agent any
	stages {
		stage('compile Stage'){
			steps {
					bat 'mvn clean compile'
			}
		}
		
		stage('Deployment Stage'){
			steps {
					bat 'mvn clean deploy -DmuleDeploy -DskipTests -Dmule.version=4.3.0 -Danypoint.username=farooq_tmc -Danypoint.password=Farooq@1054 -Denv=Sandbox -Dappname=jekins-pipeline -Dbusiness=TechMatrix-Sandbox -DvCore=Micro -Dworkers=1'
			}
		}
	}
	
	
}