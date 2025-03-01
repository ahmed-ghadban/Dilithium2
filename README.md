# Lattice-based Sign and Verify on Raspberry Pi  

This project contains an implementation of **Dilithium2**, a post-quantum digital signature scheme, running on a **Raspberry Pi**. The project measures **signing and verification times** in a real-world embedded environment, aiming to evaluate the feasibility of lattice-based cryptography for quantum-resistant security.  

## Features  
- **Dilithium Implementation**: Based on the CRYSTALS-Dilithium signature scheme. 
- **Post-Quantum Security**: Uses lattice-based cryptography to resist quantum attacks.  
- **Lightweight Application**: Designed to run efficiently on Raspberry Pi hardware.  

## Installation  

### Prerequisites  
Ensure your Raspberry Pi is set up with the necessary dependencies:  
- **Raspberry Pi 4 or 5 (any model with SSD support recommended)**  
- **Raspberry Pi OS (or a compatible Linux distribution)**  
- **4 GB ram for Raspberry Pi (recommended)**

### Clone the Repository  
```bash
git clone https://github.com/ahmed-ghadban/Dilithium2.git
cd Dilithium2
pip3 install -r requirements.txt
```

## Usage

After setting up the project, run the program with this command:
```bash
python3 Dilithium-Signature.py
```

![1000049719](https://github.com/user-attachments/assets/1945b9d4-01a8-41a1-a68f-e6cc3b226b5c)

This is the interface of the app

## Performance Evaluation

This test made on:
1. Raspberry Pi 4
2. 4 GB ram
3. ssd m.2 256GB
4. Kali Linux OS

![1000049720](https://github.com/user-attachments/assets/c402552e-c76f-4c13-9e25-79d7c4700ab6)

| Metrics | Dilithium 2 |
|:------------|:--------:|
| Sign Time      | 93.766689 mS   |
| Verify Time    | 49.124479 mS   |
| Memory usage for Key gen   | < 1.00 KB   |
| Memory usage for Signing   | < 1.00 KB |
| Memory usage for Verification | < 1.00 KB |


## References  

Refer to the [Dilithium Specification][dilithium] and [NIST PQC Project][nist] for more information.  

[dilithium]: https://pq-crystals.org/dilithium/  
[nist]: https://csrc.nist.gov/Projects/post-quantum-cryptography
