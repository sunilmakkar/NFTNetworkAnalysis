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

## How to Run the Script

1. **Download the Dataset**: First, download the dataset from Kaggle and load it into an SQLite database (e.g., `nfts.sqlite`).

2. **Update the Database Path**: In the script, make sure to update the path to the SQLite database in the `sqlite3.connect()` line:

    ```python
    con = sqlite3.connect('/path/to/nfts.sqlite')
    ```

3. **Run the Script**: After updating the database path, run the Python script:

    ```bash
    python NetworkAnalysis2.py
    ```

4. **View the Visualization**: After running the script, the output file `NFTMap.html` will be generated. You can open it in your web browser to view the network visualization.

    The visualization shows the relationships between the top NFT projects and their owners, with the size and connections of each node indicating how many NFTs they own.

## Features

- **Network Visualization**: Displays a network of NFTs, with nodes representing individual NFT projects and edges representing common ownership by wallets.
- **Top Projects and Owners**: Analyzes the top NFT projects based on transaction volume and identifies the top wallet owners.
- **Interactive Exploration**: The visualization is interactive, allowing you to explore the network by zooming, panning, and clicking on nodes to view more details.

## Customizing the Script

- **Adjusting the number of projects or owners**: You can change the number of projects or owners analyzed by modifying the `LIMIT` clause in the SQL queries within the script.
- **Graph Physics**: The `network_graph.set_options('{"physics": {"enabled": false}}')` line disables physics in the graph to prevent nodes from shaking or moving. You can enable it by changing `false` to `true`.

## License

This project is open-source and available under the MIT License.
