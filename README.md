# ⚡ QRForge — QR Code Generator

> **Create it. Scan it. Share it.**
>
> Generate QR codes for text, website URLs, Wi-Fi credentials, and contact information — instantly. Customize QR colors, preview your codes, and download them as PNG images using a lightweight, browser-based application.

---

## ✨ Features

🌐 **Multiple QR Code Types**
- Generate QR codes for plain text and messages.
- Convert website URLs into scannable QR codes.
- Create Wi-Fi connection QR codes with network names and passwords.
- Generate contact QR codes using the vCard format.
- Support hidden Wi-Fi networks and password-free networks.

⚡ **Instant QR Generation**
- Generate QR codes directly in your browser.
- Preview QR codes before downloading.
- Select from multiple image sizes.
- Customize QR code colors.
- No backend server or database required.

🎨 **Modern User Interface**
- Stylish purple glass-inspired design.
- Clean, modern, and user-friendly layout.
- Dedicated input fields for each QR code type.
- Responsive interface for desktops, tablets, and mobile devices.
- Interactive buttons and status notifications.

📥 **PNG Download**
- Download generated QR codes as PNG images.
- Choose from 200 × 200, 300 × 300, 400 × 400, and 600 × 600 sizes.
- Save QR codes for printing, sharing, or digital use.
- Generate multiple QR codes without reloading the page.

🔒 **Privacy-Friendly**
- QR content is processed locally in your browser.
- No application backend or database is required.
- No account or registration is needed.
- Wi-Fi credentials and contact details are not intentionally uploaded by the application.

---

## 📂 Project Structure

```text
QRForge-QR-Code-Generator/
│
├── index.html       ← Complete web application
└── README.md        ← Project documentation
```

The entire application is contained in a single HTML file, including the HTML structure, CSS styling, and JavaScript logic.

The QR code generation library is loaded from a CDN, so an internet connection is required for the library to load.

---

## ⚙️ Installation

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/rsamwilson2323-cloud/QRForge-QR-Code-Generator.git
```

### 2️⃣ Open the Project Folder

```bash
cd QRForge-QR-Code-Generator
```

### 3️⃣ Run the Application

Open `index.html` in any modern web browser.

**Windows users:** Double-click `index.html` to launch the application in your default browser.

✅ No installation process required.

---

## 📦 Requirements

```text
HTML5              Application structure
CSS3               Styling and responsive layout
JavaScript         QR generation and application logic
QRCode.js          QR code generation library
Modern Web Browser Chrome, Edge, Firefox, etc.
Internet           Required to load the QRCode.js CDN library
```

**No additional development dependencies are required.**

- No Node.js
- No Python
- No npm packages
- No database
- No backend server

---

## 🚀 Live Demo

You can publish QRForge using GitHub Pages after uploading the project files and enabling Pages for the repository.

**Repository:**

https://github.com/rsamwilson2323-cloud/QRForge-QR-Code-Generator

**Application file:**

https://github.com/rsamwilson2323-cloud/QRForge-QR-Code-Generator/blob/main/index.html

> To publish the website, open the repository's **Settings → Pages**, select the `main` branch and `/ (root)` folder, and save. Once GitHub Pages publishes the site, use the generated website URL to access the application.

---

## ▶️ Usage

### 📝 1. Generate a QR Code for Text

1. Open QRForge in your browser.
2. Select **Text**.
3. Enter your message in the text box.
4. Choose your preferred QR color and image size.
5. Click **Generate QR Code**.
6. Preview your QR code.
7. Click **Download PNG** to save it.

**Example input:**

```text
Hello, World!
```

The application generates a QR code that can be scanned to retrieve the original message.

### 🌐 2. Generate a Website QR Code

1. Select **Website**.
2. Enter a valid website URL.
3. Choose your preferred QR color and image size.
4. Click **Generate QR Code**.
5. Download the QR code as a PNG image.

**Example input:**

```text
https://github.com/
```

Scanning the QR code allows compatible devices to open the encoded website.

### 📶 3. Generate a Wi-Fi QR Code

1. Select **Wi-Fi**.
2. Enter the Wi-Fi network name (SSID).
3. Enter the network password if required.
4. Select the network security type.
5. Enable **Hidden network** if applicable.
6. Generate and download the QR code.

Compatible devices can scan the QR code to obtain the network connection details.

**Important:** The QR code contains the Wi-Fi credentials. Share it only with trusted people.

### 👤 4. Generate a Contact QR Code

1. Select **Contact**.
2. Enter the contact's full name.
3. Add a phone number, email address, organization, or website.
4. Choose the desired QR color and size.
5. Click **Generate QR Code**.
6. Download the resulting PNG image.

The generated contact QR code uses the vCard format, allowing compatible applications to recognize the contact information.

### 🎨 5. Customize Your QR Code

- Select a QR code color using the color picker.
- Choose an image size between 200 × 200 and 600 × 600.
- Preview the generated QR code.
- Download the final image as a PNG file.

### 🧹 6. Reset the Generator

Click **Reset generator** to clear the form, remove the generated QR code, and restore the default settings.

---

## 🧠 How It Works

### QR Code Generation

QRForge uses JavaScript and the QRCode.js library to convert the supplied content into a scannable QR code.

```text
        USER INPUT
            │
            ▼
      Select QR Type
            │
            ▼
     Validate Content
            │
            ▼
    QRCode.js Library
            │
            ▼
      Generate QR Code
            │
            ▼
       Live Preview
            │
            ▼
        PNG Download
```

### Text QR Codes

The entered text is encoded into a QR code that compatible QR scanners can read.

```text
Input:    Hello, World!
Process:  QR Code Encoding
Output:   Scannable QR Code
```

### Website QR Codes

A valid HTTP or HTTPS URL is encoded into the QR code.

```text
Input:    https://github.com/
Process:  URL Validation
Output:   QR Code Containing the URL
```

### Wi-Fi QR Codes

Wi-Fi details are formatted using a standard Wi-Fi QR payload containing the network name, security type, password, and hidden-network setting.

```text
Network:  My Wi-Fi
Security: WPA
Password: ExamplePassword
Output:   Wi-Fi Connection QR Code
```

### Contact QR Codes

Contact details are formatted using vCard 3.0, a widely supported contact data format.

```text
Name:     Sam Wilson
Phone:    +91 9876543210
Email:    sam@example.com
Output:   Contact QR Code
```

---

## 🛠️ Key Technical Details

| Feature | Implementation |
|---|---|
| Frontend | HTML5 |
| Styling | CSS3 |
| Application logic | Vanilla JavaScript |
| QR generation | QRCode.js |
| QR content types | Text, URLs, Wi-Fi, vCard |
| Color customization | HTML color input |
| Image sizes | 200, 300, 400, 600 pixels |
| Image format | PNG |
| Input validation | JavaScript |
| Download functionality | Canvas and browser download API |
| Data storage | None |
| Backend | Not required |
| Database | Not required |
| Internet connection | Required to load the CDN library |

---

## 📌 Important Notes

- QR codes store the supplied information in a machine-readable format.
- Website QR codes do not verify whether a website is trustworthy.
- Wi-Fi QR codes may contain the network password in readable form.
- Contact QR codes use the vCard format for compatibility with supported applications.
- The generated QR code should be tested with a QR scanner before printing or sharing.
- QR code colors should provide sufficient contrast for reliable scanning.
- Very long input may result in a dense QR code that is harder to scan.
- PNG downloads depend on the QR generation library loading successfully.
- The application does not require a backend, but the current CDN-based version needs an internet connection to load its QR library.
- Browser extensions, network restrictions, or security settings may affect external library loading.

---

## 🚀 Future Improvements

- 🖼️ Add custom QR code backgrounds and logos.
- 🎨 Introduce gradient colors and additional styling options.
- 📦 Support SVG downloads.
- 📚 Maintain a local history of recently generated QR codes.
- 📋 Add one-click copy functionality for generated QR content.
- 📱 Improve the mobile interface with additional customization controls.
- 🖨️ Add print-ready QR code layouts.
- 📄 Generate QR codes in bulk from CSV files.
- 🔍 Add QR code scanning and image upload support.
- 🌙 Introduce light and dark themes.
- 📊 Add QR code size and content statistics.
- 🌐 Bundle the QR library locally for fully offline operation.

---

## ⚠️ Disclaimer

This project is intended for educational, personal, and general-purpose use. It demonstrates QR code generation and browser-based web development using HTML, CSS, and JavaScript.

**QRForge generates QR codes; it does not encrypt or protect the information encoded inside them.**

Do not encode sensitive personal information or share Wi-Fi credentials with untrusted people. Always verify URLs before opening them.

---

## 👨‍💻 Author

**Sam Wilson**

🌐 GitHub: https://github.com/rsamwilson2323-cloud

💼 LinkedIn: https://www.linkedin.com/in/sam-wilson-14b554385/

---

## 📜 License

This project is distributed under the license provided in the repository's `LICENSE` file, if one is included.

---

<div align="center">

### ⚡ QRForge — QR Code Generator

**Create it. Scan it. Share it.**

*Built with HTML, CSS, and JavaScript.*

</div>
