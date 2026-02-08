🌌 Cosmic-Shield v2.0
Entropy-Driven Hybrid Encryption Suite

Cosmic-Shield is a high-integrity security tool that derives cryptographic "Roots of Trust" from the unpredictable state of the universe. By harvesting real-time telemetry of Near-Earth Objects (asteroids) from NASA's APIs, the tool ensures that encryption keys are born from true physical entropy.
🚀 Key Features

    Cosmic Entropy Harvesting: Uses real-time asteroid velocity and orbital data from NASA's NeoWs API to seed keys.

    Multi-Identity Management: Generate and manage multiple key pairs (e.g., work, personal) without overwriting data.

    Hybrid Asymmetric Architecture: * ECC (SECP256R1): For secure identity and key exchange.

        AES-256-GCM: For industrial-grade, authenticated file encryption.

    Linux Path-Safety: Fully optimized for absolute and relative paths using os.path utilities.

    Tamper Detection: Authenticated encryption ensures that any modification to the ciphertext results in a decryption failure.

🛠 Technical Stack

    Language: Python 3.x

    Crypto: cryptography.io (ECC/ECDH/HKDF), pycryptodome (AES-GCM)

    Entropy Source: NASA NeoWs (Near-Earth Object Web Service)

    Serialization: PKCS8 / X.509 PEM formats

📥 Installation & Setup

    Clone the Repo:
    Bash

    git clone https://github.com/yourusername/Real-Time-Asteroid-Telemetry-Based-Encryption-Tool.git
    cd Real-Time-Asteroid-Telemetry-Based-Encryption-Tool

    Virtual Environment:
    Bash

    python3 -m venv venv
    source venv/bin/activate

    Install Dependencies:
    Bash

    pip install -r requirements.txt

🖥 How to Use

Run the suite using:
Bash

python Tool.py

    Generate Identity: Create a named key pair (e.g., placement_key).

    Encrypt: Provide a file path and the identity name. The tool generates a .cosmic file.

    Decrypt: Provide the .cosmic file path and your identity name to recover the original file.
