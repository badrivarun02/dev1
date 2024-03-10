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
                echo 'Hello World3'
            }
        }
    }
    post{
        always{
            emailext (
                    subject: "Jenkins Build ${env.JOB_NAME} #${env.BUILD_NUMBER}",
                    body: """<p>See the attached build log for details.</p>""",
                    to: 'badrivarun09@gmail.com',
                    attachLog: true
                )
}
    }
}
