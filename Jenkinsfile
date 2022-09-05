
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                withMaven(globalMavenSettingsConfig: 'null', jdk: 'JAVA_HOME', maven: 'M2_HOME', mavenSettingsConfig: 'null') {
                    sh 'mvn clean compile'
                }
            }
        }

        stage ('Testing Stage') {

            steps {
                withMaven(globalMavenSettingsConfig: 'null', jdk: 'JAVA_HOME', maven: 'M2_HOME', mavenSettingsConfig: 'null') {
                    sh 'mvn test'
                }
            }
        }


        stage ('Deployment Stage') {
            steps {
                withMaven(globalMavenSettingsConfig: 'null', jdk: 'JAVA_HOME', maven: 'M2_HOME', mavenSettingsConfig: 'null') {
                    sh 'mvn deploy'
                }
            }
        }
    }
}
