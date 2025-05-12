# PyEscape  

A lightweight Python library for handling escape characters—sanitize, encode, decode, and manipulate strings with ease.  

---

## Features  
- **Escape/Unescape Strings**: Convert between raw and escaped strings (e.g., `\n` ↔ newline).  
- **Customizable Rules**: Define custom escape sequences or use built-in defaults.  
- **String Sanitization**: Safely escape characters for JSON, HTML, or regex contexts.  
- **Minimal Dependencies**: Pure Python with zero external dependencies.  

## Installation  
```bash
pip install pyescape  # (or your package name)
Quickstart
python
from pyescape import escape, unescape

# Escape special characters
escaped = escape("Hello\nWorld!")  # Returns "Hello\\nWorld!"  

# Unescape into raw characters
raw = unescape("Hello\\tPython!")  # Returns "Hello    Python!"  
Use Cases
Preprocessing strings for JSON/XML encoding.

Cleaning user input for secure storage.

Debugging strings with invisible escape sequences.

API Reference
escape(s: str, rules: dict = None) -> str
Escapes characters in s based on provided rules (default: \n, \t, \", etc.).

unescape(s: str, rules: dict = None) -> str
Reverts escape sequences in s to their raw characters.

Contributing
PRs welcome! See CONTRIBUTING.md for guidelines.

License
MIT
