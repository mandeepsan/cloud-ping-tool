# Cloud Ping Tool

Cloud Ping Tool is a Python-based application created to test and measure the latency (ping) between different regions of various cloud providers. This tool is essential for developers and businesses aiming to optimize application performance by selecting the most efficient cloud regions based on network latency.

## Features

- **Multi-Cloud Compatibility**: Supports multiple cloud providers, including AWS, Google Cloud, and Azure, allowing you to test pings across various regions.
- **Customizable Settings**: Easily specify which regions and providers you want to test through straightforward configuration.
- **Detailed Reporting**: Provides comprehensive latency metrics for inter-region connectivity, assisting in decision-making for cloud deployments.
- **User-Friendly**: Designed with a simple installation process and an intuitive command-line interface.

## Requirements

- Python 3.7+
- Required dependencies listed in `requirements.txt`

## Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/mandeepsan/cloud-ping-tool.git
   cd cloud-ping-tool
   ```

2. **Install the Required Packages:**

   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. **Set Up Configuration:**

   Modify the `config.json` file to specify the cloud providers and regions you are interested in testing. Here’s the configuration template:

   ```json
   {
     "providers": {
       "aws": ["us-east-1", "eu-west-1"],
       "gcp": ["us-central1", "europe-west1"],
       "azure": ["eastus", "westeurope"]
     }
   }
   ```

2. **Execute the Tool:**

   Run the script using this command:

   ```bash
   python ping_tester.py
   ```

   The script will conduct latency tests based on your configuration and will display the results in the console.

3. **Export Results:**

   To save the results to a CSV file, utilize the `--export` option:

   ```bash
   python ping_tester.py --export results.csv
   ```

## Example Command

Here's how you can run Cloud Ping Tool and export the results:

```bash
python ping_tester.py --export output.csv
```

## Contributing

Contributions are highly encouraged! If you'd like to report a bug or suggest a new feature, please open an issue. Pull requests are also welcome. Make sure your changes are well-tested and adhere to the existing code style standards.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for further details.

## Support

For any issues or questions about Cloud Ping Tool, feel free to open an issue on the GitHub repository. We aim to offer timely assistance!

## Roadmap

- Extend support for additional cloud providers.
- Develop a web-based dashboard for live data visualization.
- Enable scheduled latency tests for ongoing performance monitoring.
- Add support for cloud API authentication for private endpoint testing.

Stay updated for upcoming features and improvements!

---

We welcome any questions or feedback. Happy testing and optimizing your cloud services with Cloud Ping Tool!
