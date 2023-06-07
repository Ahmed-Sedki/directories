# Directory Discovery Tool

This Python-based tool is designed for discovering existing directories in a target URL. It automates the task of manual directory searching by providing a list of potential directories. 

## Description

The Directory Discovery Tool uses Python's `requests` library to send HTTP GET requests to the specified URL and verifies if a directory exists in that URL or not. If the tool finds an accessible directory, it will inform the user by printing out the directory's URL path. 

Please be aware that this tool should be used responsibly and ethically. It is not meant for malicious purposes such as hacking or unauthorized access to secure directories. Always get proper permission before scanning a website.

## Getting Started

### Dependencies

Make sure to install the `requests` Python library:

```
pip install requests
```

### Usage

Run the script in your Python environment and follow the on-screen instructions:

1. Enter the target URL (e.g., `www.example.com`)
2. Enter the name of the file containing the list of potential directories.

Example:
```python
python directories.py
```

### Key Components of the Code

- `request(url)`: This function sends an HTTP GET request to the URL and returns the response. If there's an error with the connection, it's handled by the `ConnectionError` exception.

- The script reads from the file containing potential directories and checks them one by one. If a valid directory is found, its full URL is printed out to the console.

### Notes

- Ensure that the file containing the list of directories is formatted correctly, with one directory per line.

- Be mindful that some websites may block your IP if you send too many requests in a short period of time. To avoid this, consider adding delays between requests.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

---

**Disclaimer:** This tool is provided for educational use only. Unauthorized scanning can lead to legal repercussions. The authors of this tool take no responsibility for misuse of the tool.
