# Telegram Bulk Account Creator

This Python script automates the process of creating bulk Telegram accounts. It leverages Selenium for browser automation, integrates proxy support, and handles account verification dynamically using a third-party service for phone numbers.

---

## Features

- **Automated Account Creation**: Automates the entire Telegram account registration process.
- **Proxy Support**: Random proxy selection from a provided proxy list.
- **Dynamic Phone Number Verification**: Integrates with a `buysim` module to handle phone number acquisition, SMS verification, and order management.
- **ChromeDriver Configuration**: Includes custom ChromeDriver options for better control of the browser instance.

---

## Requirements

### Python Dependencies
Install the required Python packages using pip:
```bash
pip install selenium
```

# Additional Requirements

- **Google Chrome**: Ensure Google Chrome is installed and matches the version of ChromeDriver.
- **ChromeDriver**: Download ChromeDriver that matches your Chrome version from [here](https://sites.google.com/chromium.org/driver/).
- **Proxies File**: A `proxies.txt` file containing proxies in the format:


# Setup

### 1. Prepare Dependencies
- Install the required Python packages.
- Place `chromedriver` in your system PATH or specify its location in `chrome_driver_configs`.

### 2. Configure Proxy File
- Create a `proxies.txt` file in the same directory as the script.
- Add your proxy list in the format: `username:password@ip:port`.

### 3. Set Configuration Files
- Ensure `configs.py` contains:
- `BASE_URL` (Telegram signup URL).
- Other necessary constants.
- Configure the `buysim` module for phone number acquisition and SMS handling.

### 4. Prepare Chrome Extensions
- Ensure `proxy_auth.py` contains the `manifest_json` and `background_js` strings for proxy configuration.

---

# Usage

Run the script from the terminal:

```bash
python account_creator.py
```