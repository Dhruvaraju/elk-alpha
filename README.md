# elk-alpha

Learning log for ELK stack

## What is ELK

- ELK is an acronym for Elasticsearch, Logstash and Kibana
- **Elastic Search** is used for store, index and analyze data
- **Logstash and Beats** are used for ingesting data into elastic search
- **Kibana** provides an user interface for this
  > Other than this we have **X-pack** which will provide seat of tools for security, Alerting, Monitoring, Reporting, Graph and also machine learning capabilities

> Elastic cloud provides all the above mentioned things in a cloud environment including x-pack

> Elasticsearch is also available in AWS(Amazon Web services), GCP (Google cloud platform), Docker and kubernetes.

## Why do you need ELK?

- Data analysis and visualization based on needs
- Which places do people visit during summer in india, you can feed in your data and add your metric. Elastic will find the patterns and provide you the possible results. Instead of we writing the entire algorithm.
- The analyzed will can be visualized by using kibana.
- X-pack is a paid product which will provide additional capabilities mentioned earlier.

## Installing ELK

- We require Java JDK for installing ELK
- Available on mac, linux, windows and docker
- in Windows navigate to elastic.co/start and download the zip files for elastic search and kibana
- Place them in a folder and extract them.
- Each folder will have a bin folder, in which you will find batch scripts for starting elastic and kibana
- once both are started open a browser and navigate to localhost:5601 you will be able to launch kibana

## Installing elastic with docker

- docker should be installed earlier
- navigate to https://www.docker.elastic.co/
- select the stack option you want to install
- pull the docker images and run them

## Elastic Search core

- to process data for generating reports based on queries or indices
- index is almost like a key based on which we run our query.
- We can create multiple indexes and run them.

## Kibana:

- Is a tool which will provide a visual representation ot the data.
- We can view data geographically, based on an index
- Can generate relation maps, pattern bar charts source and destination and many more.

## Logstash

- Used to ingest data.
- Will collect data from multiple sources and then transform it based on requirement.
- Redirect the transformed data to elastic for generating indices and reports.

## Beats

- These are also used to ingest data
- But they take a specific data and injects to elastic or logstash
- Few of the beats are mentioned below

| Name of Beat | Used for                   |
| ------------ | -------------------------- |
| Packet beat  | used for wire data         |
| File beat    | Log files                  |
| Metric beat  | used for metrics           |
| WinLogBeat   | used for windows events    |
| Audit beat   | used for audit data        |
| Heart beat   | Used for Uptime monitoring |

> Many more beats are available in the community as open source.

> If additional processing is required then the data will be streamed for Logstash else streamed to Elastic.

## X-pack

- This provide the following features
  - Security - for restricting access through passwords.
  - Monitoring - for sending alerts based on the events.
  - Reporting - generate a report and email them as an image, pdf etc.,
  - Graph - to generate graphs based on the chosen criteria.
  - Machine Learning - to find anomalies in data or do a future prediction.

> These are paid resources and the details are explained better on the website.

## Use cases for Elastic
- Log management
- Metric analysis
- Site and app searching
- Security analysis
- Application performance management

> If you are facing any issues with kibana select management tab to see index related information

> If still issues are there, you can load the projects in visual code and check the config.yml files. Check for the generated passwords are updated properly.

## Trouble shooting resources
- docs on elastic.co
- global community pages
- discuss.elastic.co
- stackoverflow