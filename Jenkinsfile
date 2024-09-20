pipeline {
    agent any
    tools {
        maven "MAVEN3"
        jdk "OracleJDK8"
    }

    environment {
        SNAP-REPO = 'vprofile-snapshot'
        NEXUS-USER = "admin"
        NEXUS-PASS = 'Afzaal@21'
        RELEASE-REPO = 'vprofile-release'
        CENTRAL-REPO = 'vpro-maven-central'
        NEXUS-GRP-REPO = 'vpro-maven-group'
        NEXUSIP = '172.31.95.117'
        NEXUSPORT = '8081'
        NEXUS-LOGIN = 'nexuslogin'
    }
    stages {
        stage('Build'){
            steps{
                sh 'mvn -s settings.xml -DskipTests install'
            }
        }
    }
}
