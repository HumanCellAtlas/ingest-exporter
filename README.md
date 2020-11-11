[![Docker Repository on Quay](https://quay.io/repository/humancellatlas/ingest-exporter/status "Docker Repository on Quay")](https://quay.io/repository/humancellatlas/ingest-demo)
[![Build Status](https://travis-ci.org/HumanCellAtlas/ingest-exporter.svg?branch=master)](https://travis-ci.org/HumanCellAtlas/ingest-exporter)
[![Maintainability](https://api.codeclimate.com/v1/badges/8c1ff877fe9c89810c14/maintainability)](https://codeclimate.com/github/HumanCellAtlas/ingest-exporter/maintainability)
[![Test Coverage](https://api.codeclimate.com/v1/badges/8c1ff877fe9c89810c14/test_coverage)](https://codeclimate.com/github/HumanCellAtlas/ingest-exporter/test_coverage)

_This repository was part of HCA DCP/1 and is not maintained anymore. DCP/2 development of this component continues in the forked repository at https://github.com/ebi-ait/ingest-exporter._

# ingest-exporter

Component that handles the generation and transmission of DSS bundles from submissions
 
This component listens for messages from the Ingest Core using RabbitMQ. When a submission is valid and complete (i.e. all data files have been uploaded to the upload area), Ingest Core will notify this component and this will generate files and bundles in the Data Store. 

```
pip install -r requirements.txt
```

```
python exporter.py
```

# testing
```
pip install -r requirements-dev.txt
```

```
nosetests
```
