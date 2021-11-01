// Powered by Infostretch 

timestamps {

node () {

	stage ('webhook-one - Checkout') {
 	 checkout([$class: 'GitSCM', branches: [[name: '*/main']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'douglasqsantos', url: 'https://github.com/douglasqsantos/webhook-one']]]) 
	}
	stage ('webhook-one - Build') {
 	
// Unable to convert a build step referring to "hudson.plugins.ansicolor.AnsiColorBuildWrapper". Please verify and convert manually if required.		// Shell build step
sh """ 
cat README.md 
 """ 
	}
}
}