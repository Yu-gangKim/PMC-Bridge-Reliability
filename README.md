# PMC Table for Bridge Reliability

This repository contains the Excel files accompanying the paper:  
**"No Simulation, in Just Seconds: A Precomputed Monte Carlo Lookup Table for Bridge Reliability"**

## Railway Bridges (`PMC_Railway_bridge_Reliability_Table_1e5x10.xlsx`)
- **SearchKey format**: `K1,V0,V1`
- **K1** : Total load effect (0.000–1.000, step 0.001)
- **V0** : COV of resistance (0.05–0.25, step 0.01)
- **V1** : COV of total load (0.05–0.25, step 0.01)
- **Example**: `652,13,05` → β = 3.1748

## Highway Bridges (`PMC_Highway_bridge_Reliability_Table_5e4x10.xlsx`)
- **SearchKey format**: `K1,K2,V0,V1,V2`
- **K1** : Dead load effect (0.00–0.80, step 0.01)
- **K2** : Vehicle load effect (0.20 to 0.80–K1, step 0.01)
- **V0** : COV of resistance (0.05–0.25, step 0.01)
- **V1** : COV of dead load (0.05–0.15, step 0.05)
- **V2** : COV of vehicle load (0.05–0.30, step 0.05)
- **Example**: `02,20,05,05,05` → β = 4.1075

## How to Use
1. Download the Excel file for your bridge type.
2. Open with Microsoft Excel.
3. Press `Ctrl+F` and enter a SearchKey in the format shown above.
4. Read the adjacent columns: `Beta_Mean`, `Beta_Std`, `Failure_Prob`.

## Contact
See the Data Availability section in the paper.
