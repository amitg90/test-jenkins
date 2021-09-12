node {
    def commit_id
    stage('Prep'){
        checkout scm
        sh "git rev-parse --short HEAD > .git/commit-id"
        commit_id = readFile('.git/commit-id').trim()
    }
//     stage('docker build/push'){
//         docker.withRegistry('https://205263170971.dkr.ecr.us-west-2.amazonaws.com',
//         'ecr:us-west-2:awsuserid'){
//              def app = docker.build("bigdataservice:bigdata-${commit_id}", '.').push()
//         }
//     }
//     stage('aws ecs'){
//         sh 'chmod +x ./awsfile.sh'
//         sh """echo ${commit_id}"""
//         sh "./awsfile.sh ${commit_id}"
//     }
}

// pipeline {
//     agent {
//         docker { image 'node:14-alpine' }
//     }
//     stages {
//         stage('Test') {
//             steps {
//                 sh 'node --version'
//             }
//         }
//     }
// }
