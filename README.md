# elk-alpha
Learning log for ELK stack
## What is ELK
- ELK is an acronym for Elasticsearch, Logstash and Kibana
- **Elastic Search** is used for store, index and analyze data
- **Logstash and Beats** are used for ingesting data into elastic search
- **Kibana** provides an user interface for this
> Other than this we have **X-pack** which will provide seat of tools for security, Alerting, Monitoring, Reporting, Graph and also machine learning capabilities

> Elastic cloud provides all the above mentioned things in a clud environment including x-pack

> Elasticsearch is also avilable in AWS(Amazon Web services), GCP (Google cloud platform), Docker and kubernetes.
## Why do you need ELK?
- Data analysis and visualization based on needs
- Which places do people visit during summer in india, you can feed in your data and add your metric. Elastic will find the patterns and provide you the possible results. Instead of we writing the entire algorithm. 
- The analyzed will can be visualized by using kibana.
- X-pack is a paid product which will provide additional capabilities mentioned earlier.

## Installing ELK
- We require Java JDK for installing ELK
- Available on mac, linux, windows and docker
- in Windows naigate to elastic.co/start and dowload the zip files for elastic search and kibana
- Place them in a folder and extract them.
- Each folder will have a bin folder, in which you will find bacth scripts for starting elastic and kibana
- once both are started open a browser and navigate to localhost:5601 you will be able to launch kibana

## Installing elastic with docker
- docker should be installed earlier
- navigate to https://www.docker.elastic.co/
- select the stack option you want to install
- pull the docoker images and run them
 
