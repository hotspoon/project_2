# Data Warehouse Project

This project is a data warehouse setup using dbt (data build tool). It includes configurations, models, macros, and tests to transform raw data into meaningful insights.

## Prerequisites

- Docker
- Python 3.7
- dbt

## Setup

1. **Clone the repository:**

   ```sh
   git clone <repository-url>
   cd <repository-directory>
   ```

2. **Build and start the Docker containers:**

   ```sh
   docker-compose up --build
   ```

3. **Set up the Python virtual environment:**

   ```sh
   cd dbt/devEnv
   python3.7 -m venv .
   source bin/activate
   pip install -r requirements.txt
   ```

4. **Configure dbt:**
   - Update the `profiles.yml` file located at [`dbt/data_warehouse/profiles.yml`](command:_github.copilot.openRelativePath?%5B%7B%22scheme%22%3A%22file%22%2C%22authority%22%3A%22%22%2C%22path%22%3A%22%2FUsers%2Ffaris%2FDocuments%2Fdigitalskola%2Fproject%2Fbelajar_docker%2Fdbt%2Fdata_warehouse%2Fprofiles.yml%22%2C%22query%22%3A%22%22%2C%22fragment%22%3A%22%22%7D%5D "/Users/faris/Documents/digitalskola/project/belajar_docker/dbt/data_warehouse/profiles.yml") with your database credentials.
   - Ensure the `dbt_project.yml` file is correctly configured.

## Running dbt

1. **Activate the virtual environment:**

   ```sh
   source dbt/devEnv/bin/activate
   ```

2. **Run dbt commands:**
   - **Initialize a new dbt project:**
     ```sh
     dbt init
     ```
   - **Run dbt models:**
     ```sh
     dbt run
     ```
   - **Test dbt models:**
     ```sh
     dbt test
     ```

## Logs

Logs are stored in the [`dbt/logs/dbt.log`](command:_github.copilot.openRelativePath?%5B%7B%22scheme%22%3A%22file%22%2C%22authority%22%3A%22%22%2C%22path%22%3A%22%2FUsers%2Ffaris%2FDocuments%2Fdigitalskola%2Fproject%2Fbelajar_docker%2Fdbt%2Flogs%2Fdbt.log%22%2C%22query%22%3A%22%22%2C%22fragment%22%3A%22%22%7D%5D "/Users/faris/Documents/digitalskola/project/belajar_docker/dbt/logs/dbt.log") file. Check this file for detailed information about the dbt operations.

## Troubleshooting

If you encounter issues with the `profiles.yml` or `dbt_project.yml` files, refer to the dbt documentation:

- [Configure your profile](https://docs.getdbt.com/docs/configure-your-profile)
- [dbt Project Configuration](https://docs.getdbt.com/docs/building-a-dbt-project/projects)

For further assistance, reach out via GitHub issues or the dbt Slack community.

Happy modeling!
