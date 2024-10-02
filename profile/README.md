# AVIS Fleet Management System

Welcome to the AVIS Fleet Management System GitHub organization. This organization contains repositories for various components of our custom fleet management webapp. The system is designed to optimize AVIS's vehicle fleet operations, including fleet composition, pricing, and sales forecasting.

## Repositories

### 1. [Web App](https://github.com/AVIS-EntropiaAI/Dashboard)
- **Description**: Next.js-based web application for visualizing and interacting with fleet management data.
- **Key Features**:
  - Real-time data visualization of fleet status and optimization results.
  - Interactive interface for running fleet optimization and price optimization models.
  - Integration with other components of the Fleet Management System.

### 2. [Fleet Composition Optimizer](https://github.com/AVIS-EntropiaAI/fleet-composition-optimizer)
- **Description**: AWS Lambda function for optimizing AVIS's vehicle fleet composition.
- **Key Features**:
  - Uses linear programming to determine optimal mix of vehicles to keep or sell.
  - Configurable constraints (budget, fleet size, minimum profit).
  - Penalty system for high mileage and aged vehicles.

### 3. [Fleet Status Updater](https://github.com/AVIS-EntropiaAI/fleet-status-updater)
- **Description**: Script for retrieving and consolidating AVIS fleet data from various sources.
- **Key Features**:
  - Combines data from databases and Excel files.
  - Provides a unified view of current fleet status.

### 4. [Price Optimization Model](https://github.com/AVIS-EntropiaAI/price-optimization-model)
- **Description**: AWS Lambda function for determining optimal selling prices for vehicles.
- **Key Features**:
  - Uses pre-trained XGBoost model to predict optimal selling price and assosciated profit.
  - Considers historical sales data and current fleet representation.

### 5. [Vehicle Categories Sales Forecast](https://github.com/AVIS-EntropiaAI/vehicle-categories-sales-forecast)
- **Description**: Python script for forecasting vehicle sales using INEGI data.
- **Key Features**:
  - Employs triple exponential smoothing (Holt-Winters method) for forecasting.
  - Optimizes model parameters for each vehicle segment.
  - Generates forecasts, metrics, and visualizations.

## Getting Started

1. Clone the desired repository:
   ```
   git clone https://github.com/AVIS-EntropiaAI/<repository-name>.git
   ```
2. Follow the setup instructions in each repository's README.md file.
3. Ensure you have the necessary permissions and credentials to access AWS services and databases as required.

## Development and Testing

- Each repository contains its own set of unit tests. Run these tests before making any changes or deployments.
- Use virtual environments when working with Python projects to manage dependencies.
- For Lambda functions, test locally using the provided instructions before deploying to AWS.

## Deployment

- Lambda functions should be deployed to your AWS environment. Ensure proper IAM roles and permissions are set up.
- For scripts, follow the usage instructions in their respective README files.
- The web app can be deployed using Vercel or your preferred Next.js hosting solution.

## Contributing

1. Fork the repository you want to contribute to.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them with clear, descriptive messages.
4. Push your changes to your fork.
5. Submit a pull request to the main repository.

## Support and Issues

If you encounter any issues or have questions, please open an issue in the relevant repository. Provide as much detail as possible, including steps to reproduce the problem and any error messages received.
