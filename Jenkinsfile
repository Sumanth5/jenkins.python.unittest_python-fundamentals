timestamps {

node () {

	stage ('first - Checkout') {
 	 checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '', url: 'https://github.com/Sumanth5/jenkins.python.unittest_python-fundamentals']]]) 
	}
	stage ('first - Build') {
 			powershell "python -m unittest discover -s ./src/test/ -p '*_test.py'"

	}
}
}
