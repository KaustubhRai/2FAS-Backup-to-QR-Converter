## Introduction
The 2FAS Backup to QR Converter is a simple and secure web application that allows you to convert your 2FAS backup files (.2fas) back into QR codes. This facilitates the easy import of your two-factor authentication (2FA) accounts into another authenticator app, (eg Google Auth, Micorsoft Auth, etc) ensuring that you maintain seamless access to your 2FA tokens.

## Features
- Drag & Drop Interface: Easily upload your .2fas backup files by dragging and dropping them into the designated area.
- File Selection: Alternatively, use the "Select File" button to browse and upload your backup files.
- QR Code Generation: Converts each 2FA account in your backup file into a QR code compatible with popular authenticator apps like Google Authenticator, Authy, and Microsoft Authenticator.
- Secure Processing: All file processing is handled locally in the browser, ensuring that your sensitive data remains private and is not transmitted over the internet.

### Live Demo

Visit - https://2fa-to-qr.netlify.app/

### How It Works
The application reads and parses the .2fas file locally in your browser.
It extracts the necessary information, such as service names, account details, and secret keys.

**QR Code Generation:**
For each 2FA account, a corresponding QR code is generated.
These QR codes can be scanned using your preferred authenticator app to set up 2FA for each service.

**Download or Save:**
Optionally, you can save or screenshot the generated QR codes for future use.

**To run locally:**

Download and install Node.js, python3
```
git clone https://github.com/KaustubhRai/2FAS-Backup-to-QR-Converter.git
cd 2FAS-Backup-to-QR-Converter
python3 -m http.server 8000
```

Open your browser and navigate to http://localhost:8000 to view the application.

Since this is a static site, there are no dependencies to install. 


### Security Considerations

- Local Processing: All file processing occurs locally in your browser. Your .2fas backup file is never uploaded or transmitted over the internet, ensuring complete privacy and security of your sensitive data.
- Content Security Policy (CSP): The application employs a robust CSP to mitigate potential cross-site scripting (XSS) attacks.
- No Data Storage: The application does not store any user data. Once the page is refreshed or closed, all processed data is cleared from the browser.

## Contributing
Contributions are welcome! Whether it's improving the UI, adding new features, or fixing bugs, your input is valuable.

