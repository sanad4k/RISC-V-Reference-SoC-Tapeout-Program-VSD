

# Week 0: VLSI System Design Program Foundation & Tool Setup

<div align="center">

![VLSI System Design](https://img.shields.io/badge/VLSI-System%20Design-blue?style=for-the-badge&logohttps://img.shields.io/badge/Week-0-orange?style=for-thehttps://img.shields.io/badge/Status-Complete-success?>

Welcome to the **VLSI System Design (VSD) Program** repository! This week focused on environment setup and installation of essential open-source EDA tools.

***

## 💻 System & VM Configuration

| Specification | Details   |
|---------------|-----------|
| OS            | Ubuntu 20.04+ |
| RAM           | 6GB      |
| Storage       | 50GB HDD |
| vCPUs         | 4        |

> 💡 *This virtual machine spec ensures smooth toolchain operation for synthesis, simulation, and layout.*

***

## ⚙️ Tool Installation & Verification

Below is the sequence of installed EDA tools and their verification screenshots, using your screenshot assets for clear documentation:

<div align="center">
GTKWave ➔ Iverilog ➔ Magic ➔ Yosys
</div>

***

### 🧠 Yosys – RTL Synthesis Tool

**Purpose:** Synthesizes Verilog RTL to gate-level netlists.

**Installation:**  
```bash
git clone https://github.com/YosysHQ/yosys.git
cd yosys  
sudo apt install make build-essential clang bison flex libreadline-dev gawk tcl-dev libffi-dev git graphviz xdot pkg-config python3 libboost-system-dev libboost-python-dev libboost-filesystem-dev zlib1g-dev
make
sudo make install
```
**Verification:**  
<p align="center">
  <img src="Screenshot_21-Sep_00-09-27_27343.jpg" alt="Yosys Installed" width="250"/>
</p>

***

### 📟 Iverilog – Verilog Simulator

**Purpose:** Compiles and simulates Verilog designs.

**Installation:**  
```bash
sudo apt-get install iverilog
```
**Verification:**  
<p align="center">
  <img src="Screenshot_21-Sep_00-09-27_27343.jpg" alt="Iverilog Installed" width="250"/>
</p>

***

### 📊 GTKWave – Waveform Viewer

**Purpose:** Visualizes simulation waveforms.

**Installation:**  
```bash
sudo apt update
sudo apt install gtkwave
```
**Verification:**  
<p align="center">
  <img src="Screenshot_21-Sep_00-09-27_27343.jpg" alt="GTKWave Installed" width="250"/>
</p>

***

### 🎨 Magic VLSI – Layout Tool

**Purpose:** IC layout editor with DRC.

**Installation:**  
```bash
sudo apt-get install m4 tcsh csh libx11-dev tcl-dev tk-dev libcairo2-dev mesa-common-dev libglu1-mesa-dev libncurses-dev
git clone https://github.com/RTimothyEdwards/magic
cd magic
./configure
make
sudo make install
```
**Verification:**  
<p align="center">
  <img src="Screenshot_21-Sep_00-09-27_27343.jpg" alt="Magic Installed" width="250"/>
</p>

***

<div align="center">

### 🎉 Installation Summary

| Tool       | Status      | Use                |
|------------|-------------|--------------------|
| 🧠 Yosys   | ✅ Complete | RTL Synthesis      |
| 📟 Iverilog| ✅ Complete | Simulation         |
| 📊 GTKWave | ✅ Complete | Waveform Analysis  |
| 🎨 Magic VLSI| ✅ Complete| Layout Editing     |

**Ready for your VLSI design journey!**

</div>

***

<div align="center">

**📂 Repository:** RTL2GDS_Alchemy  
**👨‍💻 Author:** TheVoltageVikingRam  
**📚 Program:** VLSI System Design (VSD)

</div>

***

Feel free to adjust the image tags to reference individually cropped verification screenshots. This layout makes the README more interactive and visually compelling, leveraging your attached setup screenshot across the tool sections.

[1](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/images/51217736/c5549c15-dce8-4c92-affd-89da229b641b/Screenshot_21-Sep_00-09-27_27343.jpg?AWSAccessKeyId=ASIA2F3EMEYERPIVBG34&Signature=VX266I7e4MH29oG5XZ5mh13ME%2BE%3D&x-amz-security-token=IQoJb3JpZ2luX2VjEHsaCXVzLWVhc3QtMSJIMEYCIQDuY2VZ8sTrh4qaXtpyPMOe%2FlvGjOS8LcUGitcAYYFjPQIhAL3zJWRk5fw2PDlvm%2BBog8gZf8o91f4ISqXsOeKjavl7KvoECPP%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEQARoMNjk5NzUzMzA5NzA1IgzrPIx2Kov7NN20CWsqzgRYSkUZky6ahLmAKEtdGjh4xnaDcuE%2F9KhW%2BhO0zLb56XM0NXrKulzBN1l%2BU2CWjG3rDqwNYxzbDLjYCJE9h6zvGmsrhQIiD7%2BDijOXcspsbWY9JkLqRN17L9zpm6aQhO7r1dlAEPaOCUxSCoRXmYGjMzt5rG8Yz91YU5UMxqvoSOQghAyA%2Bvc%2FanQEfJeEpsyStMD4FAgqNhOm3bxQ%2BM0tfmNaCQujYgvCsJdKPLFXftxHby%2F%2BoAnDlBbNU%2Bep%2F3qKTaq6rQTYLFTiBXIkVbMSdi6jUHuDaCMVIuI7UoJRVFoNLuHrPX9Fp7PyMPSpKcW6NMJ%2F45KiD31Zq9klwWEtYB7mfwBPFry8HciL5TV3CnezYSTEtWLMa4jc2%2BVwdxGsqOskmKt0GgJ0WBvrCCU%2F3FwnFgPsOxHYponsJIPfbqRVeQcsMFw4z4wPTQ3ZoL8LIgrvSzLCaobanpypWKtpGAk6gDSu19vpNxP0RnYj4mcwePKvrsN7xZbXsuDBry2rw%2B5eMzLQRwtn1BEz4K1GeCGfXpaRQYZfx%2F9WmLg7pJzSH%2BZ3IiYHpfE9W0uwd71ApWl1Exef4EIjumvtEwgB8pCyJUC%2B21%2Ba6Z5uExHZlcUzBG66IpDToqV6A5zsC3mYtq6UQBy%2BKjLY%2FSp69N%2BdtVpfR5elhe4e%2FhSZFz8AUnN5YZEEzXUR38iiI4Nqr%2BjP9PbNiFhPRTvtFY8EfdFr7NQ52aI5kBzLRdqicA2Ke7Q1vrNAq36KKUY22uc8PxsYDXBmCe8A4L0jd9emmjC03bvGBjqZAbnHSg8qRkrvvDvq2Xc0t4wuAZxSSq0RwhkAY2Dtw3JCccnYDKO5cfWKx4%2BvwC1gNA6ucfoBynLRl%2Fx%2BhdOXHrtrU%2Bhzoi22EQ2GxUHS6XPGCLuqdj0%2BE8zs2oXNfMI%2FPobmDBJUFQPlvysS9f0r7T38DJlVLfVp0d5fWd4b%2FhVaRfsehFIbfkTvmda90JkcowsQhaGnmSkr2A%3D%3D&Expires=1758394595)
