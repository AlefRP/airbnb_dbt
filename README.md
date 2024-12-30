# 🏠 dbt Project: Airbnb Data Modeling with Snowflake

Welcome to my dbt project! This project leverages ❄️ **Snowflake** to build and maintain an analytics-ready data warehouse for Airbnb data. It includes dimensional models, fact tables, and source data transformations.

> This project is built based on the [Complete dbt (Data Build Tool) Bootcamp: Zero to Hero](https://www.udemy.com/course/complete-dbt-data-build-tool-bootcamp-zero-to-hero-learn-dbt) by Udemy.

## 📂 Project Structure

### Models

This project includes the following types of models:

- **Source Models (`src_*.sql`)**: Raw data loaded from Airbnb datasets, used as the foundation for transformations.
- **Staging Models (`dim_*.sql`)**: Cleaned and prepared data structured into dimensions for easier querying.
- **Fact Models (`fct_*.sql`)**: Aggregated and transactional data optimized for analytical insights.
- **Intermediate Models (`dim_listings_w_hosts.sql`)**: Joins and merges of various dimensions for enhanced usability.

### File Overview

- `src_hosts.sql`: Contains the source data for hosts.
- `src_listings.sql`: Contains the source data for listings.
- `src_reviews.sql`: Contains the source data for reviews.
- `dim_hosts_cleansed.sql`: Transformed data for host details.
- `dim_listings_cleansed.sql`: Transformed data for listings details.
- `dim_listings_w_hosts.sql`: Combined data for listings and their corresponding hosts.
- `fct_reviews.sql`: Aggregated fact table for reviews data.

## 🚀 How to Use This Project

### Prerequisites

1. Ensure that Snowflake is configured and accessible.
2. Configure your `profiles.yml` with your Snowflake credentials.
3. Install dbt CLI and necessary dependencies.

### Getting Started

1. Clone this repository and navigate to the project directory.
2. Run the following commands to build and test the project:

   ```bash
   dbt run
   dbt test
   ```

### Resources

- [dbt Documentation](https://docs.getdbt.com/)
- [Snowflake Documentation](https://docs.snowflake.com/en/sql-reference/)

## ⚖️ License

This project is licensed under the [MIT License](LICENSE).