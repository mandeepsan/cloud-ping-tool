# Cloud Ping Tool

Cloud Ping Tool is a Python-based application designed to test and measure the latency (ping) between different regions of various cloud providers. This tool assists developers and organizations in optimizing application performance by identifying the most efficient cloud regions based on latency metrics.

## Features

- **Multi-Cloud Compatibility**: Supports multiple cloud providers, including AWS, Google Cloud, and Azure, enabling you to test pings across various regions.
- **Customizable Settings**: Easily configure which regions and providers you wish to test through straightforward JSON configuration.
- **Detailed Reporting**: Offers comprehensive latency metrics for inter-region connectivity, facilitating informed decision-making for cloud deployments.
- **User-Friendly**: Features a simple installation process and an intuitive command-line interface.

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

   Edit the `config.json` file to specify the cloud providers and regions you are interested in testing. Here’s a configuration template:

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

   Run the script using the following command:

   ```bash
   python ping_tester.py
   ```

   The script will conduct latency tests based on your configuration and display the results in the console.

3. **Export Results:**

   To save the results to a CSV file, use the `--export` option:

   ```bash
   python ping_tester.py --export results.csv
   ```

## Example Command

Here's how to run Cloud Ping Tool and export the results:

```bash
python ping_tester.py --export output.csv
```

## Contributing

Contributions are highly encouraged! If you'd like to report a bug or suggest a new feature, feel free to open an issue. Pull requests are also welcome. Please ensure your changes are well-tested and conform to the existing code style standards.

## License

This project is licensed under the GNU General Public License v3.0. See the [LICENSE](LICENSE) file for more details.

## Support

For any issues or questions about Cloud Ping Tool, please open an issue in the GitHub repository. We strive to provide timely assistance!

## Roadmap

- Add support for additional cloud providers.
- Develop a web-based dashboard for real-time data visualization.
- Implement scheduled latency tests for continuous performance monitoring.
- Introduce authentication support for testing private endpoints.

Stay tuned for exciting future updates and enhancements!

---

We welcome any questions or feedback. Enhance your cloud services with Cloud Ping Tool, and happy testing!
