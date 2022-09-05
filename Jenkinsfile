pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                withMaven(globalMavenSettingsConfig: 'null', globalMavenSettingsFilePath: 'C:\\Dev tools\\apache-maven-3.8.6\\conf', jdk: 'JAVA_HOME', maven: 'M2_HOME', mavenSettingsConfig: 'null', mavenSettingsFilePath: 'C:\\Dev tools\\apache-maven-3.8.6\\conf') 
   
 {
      bat 'mvn clean compile'
}
            }
        }

        stage ('Testing Stage') {

            steps {
                withMaven(globalMavenSettingsConfig: 'null', globalMavenSettingsFilePath: 'C:\\Dev tools\\apache-maven-3.8.6\\conf', jdk: 'JAVA_HOME', maven: 'M2_HOME', mavenSettingsConfig: 'null', mavenSettingsFilePath: 'C:\\Dev tools\\apache-maven-3.8.6\\conf') 
  {
     bat 'mvn test'
}
            }
        }


        stage ('Deployment Stage') {
            steps {
                withMaven(globalMavenSettingsConfig: 'null', globalMavenSettingsFilePath: 'C:\\Dev tools\\apache-maven-3.8.6\\conf', jdk: 'JAVA_HOME', maven: 'M2_HOME', mavenSettingsConfig: 'null', mavenSettingsFilePath: 'C:\\Dev tools\\apache-maven-3.8.6\\conf') 
     {
                    bat 'mvn deploy'
                }
            }
        }
    }
}
