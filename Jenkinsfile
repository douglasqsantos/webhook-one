// Powered by Infostretch 

timestamps {

node () {

	stage ('webhook-one - Checkout') {
 	 checkout([$class: 'GitSCM', branches: [[name: '*/main']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'douglasqsantos', url: 'https://github.com/douglasqsantos/webhook-one']]]) 
	}
	stage ('webhook-one - Build') {
 			// Shell build step
sh """ 
cat README.md 
 """ 
	}
}
}