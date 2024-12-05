# NFT Network Analytics

This project visualizes the relationships between NFT projects using a network graph. The analysis is based on data from Ethereum NFTs, focusing on top NFT projects and how wallets own multiple projects. The visualization uses Python, SQLite, Pandas, NetworkX, and PyVis to create an interactive network map that can be viewed in a local browser.

## Dataset

The project uses the Ethereum NFTs dataset from Kaggle. You can download the dataset from:

[Kaggle Ethereum NFTs Dataset](https://www.kaggle.com/datasets/simiotic/ethereum-nfts?resource=download)

## Project Structure

The project consists of the following:

1. **NFT Network Analysis Python Script**: This script processes the dataset and generates an interactive network visualization.
2. **NFTMap.html**: This is the output of the Python script, an HTML file with the network visualization.
3. **SQLite Database**: The dataset is loaded into a SQLite database, and the analysis script connects to it.

## Requirements

To run this project, you will need Python 3 and the following libraries:

- pandas
- sqlite3
- networkx
- pyvis

You can install the required libraries by running the following command:

```bash
pip install pandas networkx pyvis
