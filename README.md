# Network Analytics of Global Superstore Dataset

This project focuses on performing network analysis of the **Global Superstore Dataset** using various network metrics, community detection techniques, and visualization tools. The goal is to uncover insights into product-customer relationships, identify key nodes, and optimize the Global Superstore's operations by leveraging the power of network analytics.

## Project Overview

- **Objective**: To analyze the Global Superstore network and identify strategies for improving operations, inventory management, and customer engagement through network analysis.
- **Key Methods**: Centrality measures (degree, closeness, betweenness), community detection (Louvain, Girvan-Newman), and network visualization techniques.
- **Tech Stack**: Python, NetworkX, Pandas, Matplotlib, Seaborn

## Dataset

The dataset contains sales transactions from a global retail superstore. The transactions cover product categories such as office supplies, technology, and furniture, along with information on customers, sales, profit, and regions.

### Dataset Features:
- `Order ID`: Unique identifier for each order
- `Product Name`: The name of the product sold
- `Category`: Product category (e.g., Furniture, Technology, Office Supplies)
- `Customer Name`: The customer who purchased the product
- `Region`: Geographic region of the sale
- `Sales`: Sales amount for the product
- `Profit`: Profit made from the sale

### File Structure:
- **`Code.ipynb`**: Jupyter notebook containing the code for network analytics, community detection, and visualization.
- **`Code.pdf`**: PDF version of the code for easy viewing.
- **`Report.pdf`**: Detailed report discussing the methodology, network analysis results, and business insights.
- **`Global Superstore.xlsx`**: Raw Global Superstore dataset used for analysis.
- **`Global_Superstore_Preprocessed.xlsx`**: Preprocessed dataset saved after cleaning and transforming the data.
- **`requirements.txt`**: Python dependencies required to run the project.

## Model and Performance

The analysis was performed in several stages to extract insights from the network. Key results include:

### 1. Network Structure and Properties:
- **Nodes and Edges**: The network map contains 50,358 nodes and 51,179 edges.
- **Network Density**: The overall network density is 0.186, indicating moderate connectivity.
- **Disconnected Components**: Identified 1,688 disconnected components, representing isolated product-customer groups.

### 2. Community Detection:
- **Louvain Method**: The network was divided into three distinct communities based on product categories.
- **Girvan-Newman Algorithm**: Hierarchical clustering revealed more nuanced product-category relationships.
- **Key Community**: One significant community was identified around office supplies, which helped optimize marketing and product bundling strategies.

### 3. Centrality Measures:
- **Degree Centrality**: High-degree nodes, such as products like `Apple Phones` and `Cisco TelePresence`, act as hubs in the network, indicating their importance in driving sales.
- **Betweenness Centrality**: Key products like `Xerox 1916` have high betweenness centrality, bridging different product categories and serving as key drivers of cross-selling opportunities.
- **Closeness Centrality**: Identified customers with high closeness centrality, indicating those who are most influential and engaged.

## Usage

The Jupyter notebook demonstrates the following:
1. **Data Pre-processing**:
    - Cleaning the dataset and handling missing values.
    - Standardizing features for network analysis.
2. **Network Analytics**:
    - Constructing a product-customer network using `NetworkX`.
    - Computing network properties such as degree centrality, betweenness centrality, and closeness centrality.
3. **Community Detection**:
    - Using algorithms like Louvain and Girvan-Newman to detect communities and clusters in the network.
4. **Visualization**:
    - Visualizing the network structure and communities using `Matplotlib` and Gephi for detailed insights.

## Installation

To run the project locally:

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/Global-Superstore-Network-Analysis.git
    cd Global-Superstore-Network-Analysis
    ```

2. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the Jupyter notebook:
    ```bash
    jupyter notebook
    ```

## Acknowledgements

This project was developed as part of the MSc in Business Analytics at Bayes Business School.

## License

MIT License
