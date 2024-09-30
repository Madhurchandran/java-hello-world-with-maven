node {
    def mvnHome = tool 'Maven3' 

    stage('Checkout') {
        
        git credentialsId: '9ec622aa-547f-4fcd-979c-eac439d30369', url: 'https://github.com/Madhurchandran/java-hello-world-with-maven.git'
    }

    stage('Validate') {
       
        bat "${mvnHome}\\bin\\mvn validate"
    }

    stage('Clean') {
        
        bat "${mvnHome}\\bin\\mvn clean"
    }

    stage('Compile') {
       
        bat "${mvnHome}\\bin\\mvn compile"
    }

    stage('Test') {
        
        bat "${mvnHome}\\bin\\mvn test"
    }

    stage('Package') {
       
        bat "${mvnHome}\\bin\\mvn package"
    }

    stage('Verify') {
        
        bat "${mvnHome}\\bin\\mvn verify"
    }

    stage('Install') {
        
        bat "${mvnHome}\\bin\\mvn install"
    }

    stage('Site') {
        
        bat "${mvnHome}\\bin\\mvn site"
    }
}
