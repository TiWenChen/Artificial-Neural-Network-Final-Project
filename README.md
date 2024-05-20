# Artificial-Neural-Network-Final-Project

## README

### Project Overview

This project explores the integration of Gated Recurrent Units (GRUs) and Graph Attention Networks (GATs) to predict stock price movements for the constituent stocks of the 0050 ETF. By leveraging both temporal and relational data, the GRUGAT model aims to enhance the accuracy of stock return predictions.

### Key Components

1. **Graph Construction**:
   - Three types of graphs: complete, homogeneous, and heterogeneous.
     - **Complete Graph**: Includes all types of relationships (upstream, downstream, and competitive).
     - **Homogeneous Graph**: Includes only competitive relationships.
     - **Heterogeneous Graph**: Includes only supply chain relationships.
   - Each company's embedding connected to the 0050.TW node for a comprehensive market representation.

2. **Model Parameters**:
   - **GRU**: Hidden Dimension: 10, Number of Layers: 10.
   - **GAT**: Number of Layers: 2, Hidden Dimension: 10, Number of Heads: 2.

3. **Performance Analysis**:
   - Models incorporating GAT outperformed those relying solely on GRUs.
   - The homogeneous graph model showed the best accuracy in predicting cumulative returns.

### Conclusion

The GRUGAT model effectively combines temporal embeddings from GRUs with relational insights from GATs, providing a robust framework for predicting stock returns. This project highlights the significant benefits of incorporating graph-based relational data, especially in forming portfolios that outperform traditional benchmarks.

### Future Work

Future research could enhance this model by considering the dynamic nature of ETF constituent stocks and exploring additional types of inter-company relationships.

