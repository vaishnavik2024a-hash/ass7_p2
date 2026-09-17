pipeline {
 agent any
 stages {
 stage('Checkout') {
 steps {
 git branch: 'main',
 url: 'https://github.com/vaishnavik2024a-hash/ass7_p2.git'
 }
 }
 stage('Generate Result') {
 steps {
 bat 'python app.py'
 }
 }
 stage('Archive Result') {
 steps {
 archiveArtifacts artifacts: 'exam_result.txt',
 fingerprint: true
 }
 }
 }
}
