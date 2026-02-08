🌌 Cosmic-Shield: Entropy-Driven Hybrid Encryption

Cosmic-Shield is a Python-based security suite that leverages the inherent uncertainties of the universe to generate unbreakable cryptographic keys. By harvesting real-time telemetry of Near-Earth Objects (asteroids) from NASA's APIs, the tool ensures that the "root of trust" for encryption is derived from true physical entropy rather than predictable software algorithms.
🛠 Features

    Cosmic Entropy Harvesting: Uses real-time asteroid velocity and orbital data from NASA's NeoWs API to seed key generation.

    Asymmetric Identity (ECC): Implements Elliptic Curve Cryptography (SECP256R1) for secure identity and key exchange.

    Hybrid Encryption: Combines the security of ECC with the high-speed performance of AES-256-GCM.

    Authenticated Decryption: Uses GCM "Tags" to ensure file integrity—if the file is tampered with, decryption fails.

    Persistent Storage: Serializes keys into industry-standard .pem formats (PKCS8).

🚀 Technical Architecture

The tool follows the ECDH (Elliptic Curve Diffie-Hellman) key agreement protocol:

    Entropy: NASA Telemetry → SHA-256 Hash → Entropy Seed.

    Key Gen: Seed → Private Key → Public Key Allotment.

    Encryption: Ephemeral Key + Recipient Public Key → Shared Secret → AES Key → Encrypted File.

📦 Installation

    Clone the repository:
    Bash

    git clone https://github.com/yourusername/cosmic-shield.git

    Set up a virtual environment:
    Bash

    python -m venv venv
    source venv/bin/activate  # Windows: .\venv\Scripts\activate

    Install dependencies:
    Bash

    pip install -r requirements.txt

🖥 Usage

Run the main orchestrator:
Bash

python main.py

    Option 1: Generate your Cosmic Identity (creates cosmic_private.pem and cosmic_public.pem).

    Option 2: Select a file to lock using your Public Key.

    Option 3: Unlock a .cosmic file using your Private Key.
