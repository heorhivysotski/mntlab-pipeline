node('master') {
    tools {               
        env.JAVA_HOME="${tool 'java'}"
        env.PATH="${env.JAVA_HOME}/bin:${env.PATH}"
        env.GRADLE_HOME="${tool 'gradle3.3'}"
        env.PATH="${env.GRADLE_HOME}/bin:${env.PATH}"
        tool name: 'gradle3.3', type: 'gradle'
        tool name: 'java', type: 'jdk'
        tool name: 'gradle3.3', type: 'gradle' 
    }

    stage ('Preparation. Checkout') {
    git branch: 'ikhamiakou', url: 'https://github.com/MNT-Lab/mntlab-pipeline'
    }

    stage('Build') {
        sh 'gradle clean build'
   
}
