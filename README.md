# AdvancedDB-Integrity-Framework
Public (for academic sharing) 
## 📌 Overview  
A secure database framework implementing:  
- **AES-256 encryption** for data confidentiality.  
- **SHA-3 hashing** + **blockchain logging** for tamper-proof integrity.  
- **RBAC/ABAC** for granular access control.  

*(Aligns with project sections 4.1–4.4 of your report.)*  

---

## 🛠️ Setup & Installation  
### Prerequisites  
- Python 3.10+  
- PostgreSQL 14+ (or SQLite for testing)  
- Docker (optional, for blockchain simulation)  

### Steps  
1. Clone the repository:  
   ```bash
   git clone https://github.com/yourusername/AdvancedDB-Integrity-Framework.git
2. Install dependencies:
   pip install -r requirements.txt
3. Configure environment variables:
    echo "DB_PASSWORD=yourpassword" > .env
   🚀 Usage
   python
1. Encrypt Data (AES-256)
from src.encryption import encrypt_aes256

data = "Sensitive DB record"  
encrypted_data = encrypt_aes256(data)  
print(f"Encrypted: {encrypted_data.hex()}")  
2. Verify Integrity (SHA-3 + Blockchain)
from src.integrity import verify_data

is_valid = verify_data(data, blockchain_tx_id="xyz123")  
print(f"Data valid? {is_valid}")  
python -m pytest tests/
