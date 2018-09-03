pipeline {
    agent any
    
    stages {
        stage ('Create Plot from CSV') {
            steps {
                plot csvFileName: 'plot-data.csv',
                    csvSeries: [[
                        displayTableFlag: false,
                        exclusionValues: '',
                        file: 'file.csv',
                        inclusionFlag: 'OFF',
                        url: '']],
                    group: 'Spark Metrics',
                    numBuilds: '10',
                    style: 'line',
                    title: 'Spark Performance Metrics',
                    yaxis: 'Usage %',
                    yaxisMaximum: '100',
                    yaxisMinimum: '0'
            }
        }
    }
}