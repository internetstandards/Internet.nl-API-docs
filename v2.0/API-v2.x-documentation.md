# API documentation
The API documentation of the Internet.nl API v2.x can be found on https://batch.internet.nl/api/batch/openapi.yaml. 

A viewer, like ReDoc, can be used for generating a human readable version: https://redocly.github.io/redoc/?url=https://batch.internet.nl/api/batch/openapi.yaml.

Examples of API consumer scripts:
- Internet.nl Dashboard: https://github.com/internetstandards/Internet.nl-dashboard
- Internet.nl batch scripts: https://github.com/poorting/internet.nl_batch_scripts

# Sequence of handling batches of domains
- Batch requests are processed on a FIFO basis for a particular user. This means a users can submit multiple batch requests, but they are processed sequentally. The first / current batch requests needs to finish before the next one starts. 
- Batch requests of multiple users are run in parallel. While influenced by the number of users running simultaneous batch requests, you should assume that parallel tasks take longer to finish since server resources are being shared. 
