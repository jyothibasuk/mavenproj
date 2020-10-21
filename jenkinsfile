node() {

    stage(" git download ") {
    	checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/jyothibasuk/mavenproj.git']]])
    }

    stage(" Build ") {
        sh 'mvn package'
    }
}
