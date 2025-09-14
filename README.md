

# DDoS Detection and Mitigation in SDN

This project is a Python-based DDoS attack detection and mitigation system built using Ryu controllers and Mininet for Software-Defined Networking (SDN).

-----

## Description

This repository contains a solution for detecting and mitigating Distributed Denial of Service (DDoS) attacks within an SDN environment. The system monitors network traffic, identifies anomalous patterns indicative of a DDoS attack, and then applies mitigation techniques to block the malicious traffic while allowing legitimate traffic to pass through.

-----

## Features

  * **Real-time Traffic Monitoring**: Continuously monitors network traffic for suspicious activity.
  * **DDoS Attack Detection**: Utilizes machine learning and statistical analysis to detect DDoS attacks.
  * **Automatic Mitigation**: Implements flow rules to block or limit traffic from attacking sources.
  * **Customizable Topologies**: Allows for the creation of custom network topologies using Mininet.

-----

## Technologies Used

  * **Python**
  * **Ryu SDN Controller**
  * **Mininet**
  * **OpenFlow**
  * **Scikit-learn**

-----

## Getting Started

### Prerequisites

  * Ubuntu 20.04 or later
  * Python 3.8 or later
  * Mininet
  * Ryu SDN Framework

### Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/Ajajay44/ddos-detection-and-mitigation.git
    cd ddos-detection-and-mitigation
    ```
2.  **Install the required Python packages:**
    ```bash
    pip install -r requirements.txt
    ```

-----

## Usage

1.  **Run the Ryu controller with the DDoS detection application:**
    ```bash
    ryu-manager DDOS_Attack_Detection_Mitigation-master/controller/KNN_controller.py
    ```
2.  **In a separate terminal, start the Mininet topology:**
    ```bash
    sudo python topology.py
    ```
3.  **To simulate a DDoS attack, you can use a tool like `hping3`:**
    ```bash
    sudo hping3 -S --flood -V <target_ip>
    ```

-----

## Contributing

Contributions are welcome\! Please feel free to submit a pull request or open an issue to discuss your ideas.

-----

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.
