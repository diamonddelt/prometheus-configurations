# Prometheus Configurations

Various Prometheus configurations and setup for various setups and situations

## Windows Localhost (General Purpose)

### Prerequisites

1. Install prometheus and put the binary on the PATH
2. Install [wmi_exporter](https://github.com/martinlindhe/wmi_exporter/releases)
3. Configure `prometheus-win.yml` to point to whatever port you have wmi*exporter exposing (default is \_9182*)
4. View the generated prometheus time-series data at `localhost:9090`

## Sample Windows metrics to monitor

### Network

- `wmi_net_bytes_received_total`
- `wmi_net_current_bandwidth`
- `wmi_net_packets_received_errors`
- `wmi_net_packets_outbound_errors`
