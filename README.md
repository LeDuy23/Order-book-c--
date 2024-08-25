# Order book 


Order Book Implementation in C++

Overview

This project is a C++ implementation of an Order Book, a core component of trading platforms in financial markets. The order book efficiently manages buy and sell orders, matches them based on price and time priority, and simulates the trading process. This project showcases skills in C++ programming, data structure optimization, and real-time trading logic.

Features

1. Order Management
Buy and Sell Orders: The system handles and processes incoming buy and sell orders.
Order Types: Supports different types of orders:
Market Orders: Executed immediately at the best available price.
Limit Orders: Executed at a specified price or better.
FillOrKill Orders: These orders must be filled entirely immediately or canceled (killed) without any partial fills.
GoodForDay Orders: These orders remain active until the end of the trading day or until they are executed, whichever comes first.
Order Matching: Automatically matches orders based on price and time priority.
2. Data Structures
Efficient Storage: Orders are stored using optimized data structures, such as maps or priority queues, for quick access and updates.
Price Levels: The order book is organized by price levels, each containing a list of orders at that specific price.
3. Trading Logic
Price-Time Priority: Orders are matched based on the best price and the earliest time of arrival if prices are the same.
Partial Fills: Supports partial order fills, allowing orders to be partially executed if there isn't enough quantity at a given price level (except for FillOrKill orders).
4. Unit Testing
Google Test Framework: The project includes comprehensive unit tests written using the Google Test framework. These tests validate the correctness of the order matching logic, data structures, and overall functionality.

