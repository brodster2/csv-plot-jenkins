pipeline {
    agent any
    
    stages {
        stage ('Create Plot from CSV') {
            steps {
                plot csvFileName: 'plot-8e7e56f2-ead7-4330-a646-a69c55dc0131.csv',
                    csvSeries: [[
                        displayTableFlag: false,
                        exclusionValues: '',
                        file: 'data.csv',
                        inclusionFlag: 'OFF',
                        url: '']],
                    group: 'Spark Metrics',
                    numBuilds: '10',
                    style: 'line',
                    title: 'Spark Performance Metrics',
                    yaxis: 'Metric Type',
                    yaxisMaximum: '100',
                    yaxisMinimum: '0'
            }
        }
    }
}