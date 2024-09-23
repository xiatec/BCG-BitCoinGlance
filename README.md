# BitcoinMonitor: Real-time Cryptocurrency Exchange Data Pipeline

## Project Overview

BitcoinMonitor is a robust, scalable data engineering solution designed to capture, process, and analyze real-time cryptocurrency exchange data. This project demonstrates proficiency in building end-to-end ETL pipelines, data warehousing, and creating actionable insights for financial analysis.

## Key Features

1. **Real-time Data Ingestion**: Automated ETL process pulling live data from the CoinCap API every 5 minutes.
2. **Scalable Data Warehouse**: Utilizes PostgreSQL for efficient storage and querying of large-scale financial data.
3. **Containerized Architecture**: Docker-based setup ensuring consistency across development, testing, and production environments.
4. **Automated Testing**: Comprehensive unit and integration tests to maintain data integrity and pipeline reliability.
5. **Infrastructure as Code**: Terraform scripts for easy deployment and management of AWS infrastructure.
6. **Data Visualization**: Integrated Metabase dashboard for real-time market insights and trend analysis.

## Technology Stack

- **ETL Pipeline**: Python, requests library
- **Data Warehouse**: PostgreSQL
- **Containerization**: Docker, Docker Compose
- **Scheduling**: Cron
- **Cloud Infrastructure**: AWS EC2, Terraform
- **Testing**: pytest
- **Code Quality**: Black, Flake8, MyPy, isort
- **Data Visualization**: Metabase

## Business Value

1. **Market Intelligence**: Provides up-to-the-minute insights on cryptocurrency exchange performance, enabling informed trading decisions and strategy formulation.
2. **Risk Management**: Allows financial institutions to monitor market volatility and adjust their cryptocurrency portfolios in real-time.
3. **Competitive Analysis**: Offers a comprehensive view of trading volumes and market share across different exchanges, facilitating competitive benchmarking.
4. **Operational Efficiency**: Automates data collection and processing, reducing manual effort and minimizing human error in financial data analysis.
5. **Scalability**: Designed to handle increasing data volumes as the cryptocurrency market expands, ensuring long-term viability.

## Data Engineering Highlights

1. **Efficient ETL Design**: Optimized Python scripts for extracting and transforming large volumes of financial data with minimal latency.
2. **Data Quality Assurance**: Implemented robust error handling and data validation to ensure the accuracy and reliability of financial metrics.
3. **Performance Tuning**: Optimized PostgreSQL queries and table structures for fast data retrieval, essential for real-time financial analysis.
4. **Scalable Architecture**: Designed a modular, containerized system that can easily scale to accommodate additional data sources or increased data volumes.
5. **DevOps Integration**: Incorporated CI/CD practices with automated testing and infrastructure-as-code, demonstrating a modern approach to data engineering.

## Running the Pipeline

To run the BitcoinMonitor pipeline, follow these steps:

1. Clone the repository:
   ```
   git clone https://github.com/your-username/bitcoinMonitor.git
   cd bitcoinMonitor
   ```

2. Set up environment variables:
   Copy the `.env.example` file to `.env` and fill in the necessary credentials.

3. Build and start the Docker containers:
   ```
   make up
   ```

4. Run database migrations:
   ```
   make warehouse-migration
   ```

5. To stop the pipeline:
   ```
   make down
   ```

6. To run tests:
   ```
   make pytest
   ```

7. To check code quality:
   ```
   make ci
   ```

For more detailed commands, refer to the Makefile:
