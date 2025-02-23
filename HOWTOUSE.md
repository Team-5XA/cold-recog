# Cold-Recog - How to Use

## Installation Instructions

### Step 1: Download the source code from the github
1. Visit the [GitHub ](https://github.com/team-5XA/cold-recog) page for Cold-Recog.
2. Download the latest version of the plugin as a `.zip` or  file.
3. Since Cold Recog contains submodules, you need to initialize them properly after cloning. Follow these steps:</br>
    1️⃣ Clone the Repository (Including Submodules)
    ```sh
    git clone --recurse-submodules https://github.com/team-5XA/cold-recog.git
    cd cold-recog
    ```
    2️⃣If You Already Cloned It (Without Submodules)

    If you forgot to include `--recurse-submodules`, run:
    ```sh
    git submodule update --init --recursive
    ```
    3️⃣(Optional) If a Submodule Isn't Working Properly

    Reset and reinitialize:
    ```sh
    git submodule deinit -f .
    git submodule update --init --recursive
    ```

## **Installation Guide**

### **🔹 1. Frontend Setup (React)**
**Requirements:** Node.js (v18+)

#### **Install Dependencies**
```sh
cd cr-frontend
npm install
```

#### **Start the Development Server**
```sh
npm start
```
**Default URL:** `http://localhost:3000`

---

### **🔹 2. Backend Setup (Custom API/ Flask)**
**Requirements:** Python 3.10+, pip, virtual environment

#### **Install Dependencies --- > Automation Script**
```sh
cd cr-backend
chmod+x setup.sh
./setup.sh
python app.py
```

#### **Install Dependencies --- > Manual**
```sh
cd backend
python -m venv venv
source venv/bin/activate   # macOS/Linux
venv\Scripts\activate      # Windows
pip install -r requirements.txt
```

**Default URL:** `http://localhost:5000`

---


## Usage

1. **Run the Flask application**:

   ```bash
   python app.py
   ```

2. **Upload an image**:

   Use the /upload endpoint to upload an image and find matches.

   Example using curl:

   ```bash
   curl -X POST -F "file=@path_to_your_image.jpg" http://localhost:5000/upload
   ```

   Retrieve matched images:

   Use the `/matched-images/<filename>` endpoint to retrieve matched images.

   Example using curl:

   ```bash
     curl -O http://localhost:5000/matched-images/matched_image.jpg
   ```

### API Endpoints:

```
    POST /upload: Upload an image to find matching faces.
	Request: Form-data with a file field named file.
	Response: JSON with matched images data or an error message.

	GET /matched-images/<filename>: Retrieve a matched image by filename.
       Response: The matched image file or an error message.
```

Example Response:

```json
{
  "matched_images": [
    {
      "file_name": "matched_image1.jpg",
      "distance": 0.45,
      "match_rate": 45.0
    },
    {
      "file_name": "matched_image2.jpg",
      "distance": 0.5,
      "match_rate": 50.0
    }
  ]
}
```

### Configuration :

    MATCHED_IMAGES_DIR: Directory to save matched images temporarily.
    DATASET_DIR: Directory containing the dataset images.---

## Notes and Best Practices

  - Always ensure data privacy by anonymizing sensitive information before processing.
  - Regularly update the AI model to improve accuracy and minimize bias.
  - Follow secure coding practices to prevent vulnerabilities and unauthorized access.

## Troubleshooting 
  - Backend not starting? → Verify dependencies with pip list and ensure the correct Python version is used.
  - CORS issues? → Verify backend allows requests from http://localhost:3000.
  - Frontend not loading properly? → Try clearing cache and restarting:
      ```sh
      rm -rf .next node_modules package-lock.json
      npm install
      npm start
      ```
  - Still getting errors? → Use Postman or cURL to manually test API requests with headers.

 ## Support
 
For further assistance, please visit the [Cold-Recog GitHub Repository](https://github.com/team-5XA/cold-recog) or contact support at `fivexa69@gmail.com`.
