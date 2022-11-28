# Grafana_Performance_Comparison

This Grafana dashboard gives you a comparison of performance results between any 2 past runs.

- I'm using this backend listener 1.2.2 which writes 100% results to InfluxDb: https://sfakrudeen78.github.io/JMeter-InfluxDB-Writer/

- When you add backend listener into the test plan, specify a unique string to the runId field e.g. timestamp or any unique name because that value unqiuely identifies a test and groups all stats based on this value. e.g. I have used ${__time(yyyy-MM-dd_HHmm,)}

- Just import the json into Grafana and create a new dashboard. May need to change some SQL's to amend the jmeter sampler names

- This dashboard assumes, inFluxDB is your default datasource.

- Please change the variable values from dashboard settings after importing the json

![IMG_0984](https://user-images.githubusercontent.com/19985725/174286984-1d114fff-da36-4040-9cd4-3a54b6a16196.jpeg)

