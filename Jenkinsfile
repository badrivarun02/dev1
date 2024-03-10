pipeline {
    agent any

    stages {
        stage('clone repositor'){
            steps {
              git branch: 'main', url:'https://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@github.com/badrivarun02/dev1.git'
           }
        }
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
    }
}
