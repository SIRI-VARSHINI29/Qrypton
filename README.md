## 🔐 Qrypton: Advanced Encryption for Quantum-Safe Video Transmission

## 🧩 Introduction
Qrypton is a secure, Flask-based web application built to protect video content through encryption, watermarking, and Shamir’s Secret Sharing. It offers a complete framework for uploading, processing, encrypting, and reconstructing videos in a user-friendly way, ensuring quantum-safe video transmission.

By integrating advanced cryptography and video processing techniques, Qrypton enables data privacy, content authenticity, and controlled access to sensitive video files.


## 🌟 Key Features

- 🔑 User authentication system (Register/Login)  
- 📤 Upload videos with custom watermarks  
- 🔐 Video encryption using `cryptography`  
- 🧩 Key splitting using Shamir's Secret Sharing  
- 📦 Secure storage of encrypted frames  
- 🔓 Decrypt using collected key shares  
- 🎬 Watermark recovery from first frame  
- 📥 Download decrypted videos  


## 🛠 Technologies Used

The **Qrypton** project leverages:

- **Flask**: Serves as the backend framework to handle routes, forms, and HTTP requests.
- **OpenCV**: Processes videos frame by frame and embeds/extracts watermarks.
- **Cryptography**: Encrypts each video securely using AES or similar algorithms.
- **Shamir’s Secret Sharing**: Splits the encryption key into multiple shares for secure reconstruction.
- **HTML/CSS/JS**: Designs a responsive and clean user interface.
- **Jinja2**: Handles dynamic content rendering in templates.
- **Python Standard Libraries**:
  os, uuid, shutil for directory and file operations
  base64, io for encoding and decoding secure content.


## ✅ Prerequisites
To set up and run Qrypton, ensure the following:

1.Python 3.8+ installed

2.Required libraries installed:
```bash
pip install flask opencv-python cryptography
```

3.Create the following folders in the root directory if not present:
```bash
mkdir uploads shares decrypted
```

## ⚙️ How to Run
1. Clone the repository or download the project files:
```bash
git clone https://github.com/YOUR_USERNAME/qrypton.git

cd qrypton
```
2.Install dependencies:
```bash
pip install -r requirements.txt
```

3.Run the Flask app:
```bash
python app.py
```

## 🔄 Use Flow

1. **Register or log in.**

2. **Upload a video and watermark image.**

3. **The system performs the following steps:**
   - Splits video into frames  
   - Embeds watermark into each frame  
   - Encrypts each frame  
   - Splits the encryption key into secure shares

4. **Download** the encrypted video or **reconstruct** it by uploading valid key shares.

5. **Extract** the watermark from the first decrypted frame.

   

## 🚧 Future Enhancements

- Real-time video encryption and live streaming support  
- Blockchain-based logging for audit and verification  
- Multi-factor authentication  
- Cloud integration (AWS/GCP/Drive)  
- Advanced watermarking with invisible or AI-generated signatures  
- Role-based user access and admin panels

## 📚 References
This project is built on research and techniques in post-quantum cryptography and secure multimedia processing.


