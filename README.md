# Clustering Project for Branch Selection

## Problem Statement Summary

Company X aims to expand its business in Egypt by opening new branches at recommended locations categorized as Location A and Location B. The company seeks to select a subset of branches for maximum coverage and sales without any loss. 

- Location A: Operational costs of $25,000 with 2536 recommendations.
- Location B: Operational costs of $15,000 with 134 recommendations.
- Sales data available only for Location A branches.
- Assumption: Any branch can cover the sales of another branch within 5 km.

## Approaches to Solve the Problem

### Approach 1
1. Calculate haversine distance between Location A branches.
2. Estimate sales based on branches within 5 km.
3. Filter branches where estimated sales > operational costs.
4. Select non-overlapping branches.

### Approach 2
1. Combine Location A and Location B data.
2. Use Ball Tree to assign neighbors.
3. Cluster points and calculate estimated sales.
4. Retain points with sales > costs.

### Approach 3
1. Combine Location A and Location B data.
2. Cluster using DBSCAN.
3. Calculate estimated sales for each cluster.
4. Retain points with sales > costs and non-overlapping.

### Approach 4
1. Combine Location A and Location B data.
2. Cluster using HDBSCAN.
3. Calculate estimated sales for each cluster.
4. Retain points with sales > costs and non-overlapping.

Feel free to explore the code and datasets provided in this repository for detailed implementation and results.
