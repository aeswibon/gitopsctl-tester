# GitOpsCTL Tester Repository

This repository is designed to serve as a testing ground for validating the functionality of [GitOpsCTL](https://github.com/aeswibon/gitopsctl), a tool for managing GitOps workflows. It contains various Kubernetes YAML manifests that can be used to test and verify different features and scenarios supported by GitOpsCTL.

## Purpose

The primary purpose of this repository is to:

- Provide a collection of Kubernetes YAML manifests for testing GitOpsCTL functionality.
- Simulate real-world scenarios to ensure GitOpsCTL behaves as expected.
- Serve as a reference for troubleshooting and debugging GitOpsCTL workflows.

## Repository Structure

The repository is organized as follows:

- **manifests/**: Contains Kubernetes YAML manifests for testing various configurations and use cases.
- **scripts/**: Includes helper scripts for automating tests or setting up environments.
- **docs/**: Additional documentation related to testing scenarios and configurations.

## Getting Started

To use this repository for testing GitOpsCTL:

1. Clone the repository:

   ```bash
   git clone https://github.com/aeswibon/gitopsctl-tester.git
   cd gitopsctl-tester
   ```

2. Ensure you have GitOpsCTL installed. Refer to the [GitOpsCTL documentation](https://github.com/aeswibon/gitopsctl) for installation instructions.

3. Apply the Kubernetes manifests using GitOpsCTL:

   ```bash
   gitopsctl register \
   --name my-nginx-app \
   --repo https://github.com/aeswibon/gitopsctl-tester.git \
   --path manifests \
   --kubeconfig ~/.kube/config \
   --interval 30s
   ```

4. Verify the results and debug any issues using the logs or GitOpsCTL commands.

## Contributing

Contributions are welcome! If you have additional test cases or scenarios, feel free to submit a pull request. Please ensure your changes are well-documented and follow the repository structure.

## License

This repository is licensed under the [MIT License](LICENSE). Feel free to use and modify the contents for your own testing purposes.

## Contact

For questions or issues related to this repository, please reach out via the [GitOpsCTL project](https://github.com/aeswibon/gitopsctl) or open an issue in this repository.
