# Base Package

This is a [Kurtosis][kurtosis-repo] package developed by [LZero](https://www.lzeroanalytics.com), which allows you to deploy a private Layer 2 Base network on top of the Ethereum Layer 1 testnet.

## Quickstart

1. [Install Docker & start the Docker Daemon if you haven't done so already][docker-installation]
2. [Install the Kurtosis CLI, or upgrade it to the latest version if it's already installed][kurtosis-cli-installation]
3. Run the package with default configurations from the command line:
   
   ```bash
   kurtosis run --enclave my-testnet github.com/LZeroAnalytics/base-package
   ```

#### Run with your own configuration

Kurtosis packages are parameterizable, meaning you can customize your network and its behavior to suit your needs by storing parameters in a file that you can pass in at runtime like so:

```bash
kurtosis run --enclave my-testnet github.com/LZeroAnalytics/base-package --args-file network_params.yaml
```

Where `network_params.yaml` contains the parameters for your network in your home directory.

<!------------------------ Only links below here -------------------------------->

[docker-installation]: https://docs.docker.com/get-docker/
[kurtosis-cli-installation]: https://docs.kurtosis.com/install
[kurtosis-repo]: https://github.com/kurtosis-tech/kurtosis