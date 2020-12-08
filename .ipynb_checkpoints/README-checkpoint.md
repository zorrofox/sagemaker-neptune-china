# SageMaker Neptune Setup in China Region

## Prerequisite

- Create a Neptune database in Ningxia Region, please following the [AWS guide](https://docs.amazonaws.cn/neptune/latest/userguide/get-started.html)
- Get all the Neptune database cluster information:
  - Cluster endpoint
  - Reader endpoint
  - Port
- Create a SageMaker Notebook instance follow [this guide](https://docs.amazonaws.cn/sagemaker/latest/dg/howitworks-create-ws.html), and pelase ensure these:
  - the SageMaker notebook instance and Neptune database need in one VPC
  - the Neptune Security Group need let SageMaker notebook instance access

## Setup SageMaker Notebook Instance
- Check out this Github repository in your Notebook instance
- Open notebook [setup.ipynb](setup.ipynb), run the cells follow the Notebook guide.

## Testing Neptune Setup
- Open the folder `gremlin-training-imdb` and follow the notebooks guide to test the Neptune setup.