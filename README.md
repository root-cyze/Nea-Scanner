# Nea Scanner

![IMG_20250526_063530~2](https://github.com/user-attachments/assets/59d2d868-042a-432e-8a86-e4d62ef96b49)



**Nea Scanner** is a high-performance, asynchronous web directory scanner built using modern Python technologies like `aiohttp` and `asyncio`. It efficiently discovers hidden directories and files on web servers with customizable wordlists.

## Features

- Asynchronous scanning with `aiohttp` for high speed
- HTML title extraction for better insights
- Response details: status code, content length, type, server header, redirect location
- Custom wordlist support
- Proxy support and adjustable request delay
- Auto-generated default wordlist if none is provided
- Exports results in JSON, CSV, or TXT format
- Colored terminal output for better readability

## Installation

```
git clone https://github.com/root-cyze/Nea-Scanner.git
```
```
cd nea-scanner
```
```
pip install -r requirements.txt
```
> Requirements: Python 3.7+, aiohttp, aiofiles

Run the scanner:
```
python3 scanner.py
```
You will be prompted to enter the following:
`
Target URL (with http:// or https://)
`
Wordlist file path (or leave blank to use the default)
`
Number of concurrent requests
`
`
Delay between requests (in seconds)
`
Timeout duration
`
Optional proxy URL (e.g. http://127.0.0.1:8080)
`
Output file path and format (json, csv, or txt)


Example
`
python3 scanner.py
`
Sample inputs:
```
Enter target URL: http://example.com
Enter wordlist path: wordlist.txt
Concurrent requests (default 50): 100
Delay (default 0): 0
Timeout (default 10): 10
Proxy (leave blank for none): 
Output file (optional): results.json
Output format (json/csv/txt, default json): json

Output

The scanner provides output in the terminal as well as optionally saving to a file:

JSON: Structured data, good for further analysis or integration

CSV: Easily viewable in spreadsheet software

TXT: Human-readable log-style output
```
# File Structure

├── scanner.py   
├── wordlist.txt       
└── README.md              

---
# License

MIT License


---

Nea Scanner was developed for educational and security testing purposes. Always get proper authorization before scanning any target.

---
