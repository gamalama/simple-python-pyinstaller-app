node {
    docker.image('python:2-alpine') {
        stage('Build') {
            checkout scm
            sh 'python -m py_compile sources/add2vals.py sources/calc.py'
        }
    }
    // docker.image('qnib/pytest') {
    //     stage('Test') {
    //         sh 'py.test --verbose --junit-xml test-reports/results.xml sources/test_calc.py'
    //     }
    // }
}
