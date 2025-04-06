# LocalPhish

A web-based social engineering tool for educational purposes only.


Star⭐ the repo if you like what you see😉.
<p align="center">
  <a href="https://github.com/localsix/Localpish/"><img alt="Star" src="https://img.shields.io/github/stars/localsix/Localpish"></a>
</p>

![Screenshot (1121)](https://github.com/user-attachments/assets/2745ab93-958b-4476-9a47-b4e77250a720)

![Screenshot (1120)](https://github.com/user-attachments/assets/c3873159-acad-4d89-a711-9e0206e0c9b1)

![Screenshot (1119)](https://github.com/user-attachments/assets/e8ce18c2-57f1-4d10-8365-a690385cf404)

![ddaffv](https://github.com/user-attachments/assets/d6ad25d1-e30f-48bd-a0bf-6aaf092e7352)

![Screenshot (1114)](https://github.com/user-attachments/assets/3b3c9dad-779d-47b3-a8dc-f9113256e366)


**THIS TOOL IS FOR EDUCATIONAL PURPOSES ONLY**

This tool is provided for educational and research purposes only. Using this tool against targets without explicit mutual consent is illegal. The developers assume no liability and are not responsible for any misuse or damage caused by this program.

only run in windows environment

## Features

### Core Functionality
- Clone Website directly from url 
- Tunneling
- HTTP Server & Data Intercept
- Credential Logging
- Redirect System
- Bypass Cloudflare Turnstile (removed for this tool project)

### Technical Features
- **Multi-method Template Fetching:**
  - Selenium-based fetching with Chrome WebDriver
  - Anti-detection mechanisms (random delays, user agent rotation)
  - Proxy-based fetching as fallback
  - Manual template selection option
- **Resource Path Fixing:** Automatically corrects relative paths in cloned websites
- **Multiple Tunneling Options:**
  - Ngrok integration for public access
  - Localhost option for testing
- **Robust Error Handling:** Fallback systems when primary methods fail

### Security Features
- **Save File Validation:** Ensures the capture file is writable before starting
- **CloudFlare/CAPTCHA Detection:** Identifies and attempts to handle anti-bot protections (Remove in project)
- **Cookie Storage:** Saves cookies for potential authenticated sessions
- **Comprehensive Data Capture:** Saves all form fields, not just credentials

### Cross-Platform Support
- **Windows Optimization:** Specifically designed for Windows environments
- **Automatic Tool Installation:** Downloads required external tools (Ngrok)

## Installation

### Prerequisites

- Python 3.6 or higher
- Internet connection for dependency installation
- Windows OS (some modifications required for other OS)

### Setup

1. Clone the repository:
```
git clone https://github.com/localsix/Localpish.git
cd Localpish
```

2. Install required dependencies:
```
pip install -r requirements.txt
```

## Usage

1. Run the script:
```
python localphish.py
```

2. Follow the interactive prompts:
   - Set your target URL (where victims will be redirected after login)
   - Choose whether to automatically fetch the login template from the target site
   - Select a tunneling method (Ngrok recommended for public access)

3. Once the server is running, you'll get a URL to share with your targets. All captured credentials will be saved to `save.txt` in the script directory.

## Tunneling Options

### NGROK
- Requires free registration at [ngrok.com](https://ngrok.com)
- Provides a public URL accessible from anywhere
- You will need to provide your Ngrok authtoken when prompted

### LOCALHOST ONLY
- For testing purposes only
- Only accessible on your local machine

## Technical Details

### Directory Structure
- `.tmp/` - Temporary directory for website templates
- `save.txt` - File where captured credentials are saved

## Troubleshooting

### Common Issues

1. **Ngrok not working**
   - Ensure your authtoken is correct
   - Check if port 4040 is accessible
   - Verify your firewall isn't blocking Ngrok

2. **Template fetching fails**
   - Try providing a manual HTML template
   - Check your internet connection
   - Some sites may have anti-bot protections

3. **Permission errors**
   - Run the script with appropriate permissions
   - Ensure the directory is writable

## Contact

- Discord: localsix66
- GitHub: [localsix](https://github.com/localsix)

## License

This project is licensed under the MIT License - see the LICENSE file for details.
