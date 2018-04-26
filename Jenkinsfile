pipeline {
    agent any

    stages {
        stage ('Compile Stage') {
            bat 'mvn verify'  
         }

        stage ('Testing Stage') {
            cucumber fileIncludePattern: '**/*.json', sortingMethod: 'ALPHABETICAL'
        }
    }
}
