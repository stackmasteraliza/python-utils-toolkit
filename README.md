# Python Utils Toolkit

A collection of reusable Python utility scripts to help with everyday tasks. This project is designed to grow with daily contributions and improvements.

## Project Structure

```
python_utils_toolkit/
├── utils/
│   ├── __init__.py
│   ├── file_utils.py      # File operations (copy, move, rename, search)
│   ├── text_utils.py      # Text processing (parse, format, validate)
│   ├── date_utils.py      # Date/time operations
│   ├── web_utils.py       # Web utilities (download, scrape, API helpers)
│   └── system_utils.py    # System utilities (disk space, process info)
├── examples/
│   └── demo_scripts.py    # Example usage of utilities
├── tests/
│   └── test_utils.py      # Unit tests
├── requirements.txt
└── README.md
```

## Installation

```bash
# Clone the repository
git clone <your-repo-url>
cd python_utils_toolkit

# Install dependencies
pip install -r requirements.txt
```

## Utilities Overview

### File Utilities (`utils/file_utils.py`)
- `find_files()` - Search files by pattern
- `get_file_info()` - Get file metadata
- `batch_rename()` - Rename multiple files
- `find_duplicates()` - Find duplicate files
- `organize_by_extension()` - Organize files by type

### Text Utilities (`utils/text_utils.py`)
- `extract_emails()` - Extract emails from text
- `extract_urls()` - Extract URLs from text
- `word_frequency()` - Count word occurrences
- `slugify()` - Convert text to URL-friendly slug
- `validate_email()` - Validate email format

### Date Utilities (`utils/date_utils.py`)
- `time_ago()` - Human-readable time difference
- `business_days_between()` - Calculate business days
- `format_duration()` - Format seconds to readable duration
- `get_week_dates()` - Get all dates in a week

### Web Utilities (`utils/web_utils.py`)
- `download_file()` - Download file with progress bar
- `is_url_valid()` - Check if URL is accessible
- `get_page_title()` - Get webpage title
- `shorten_url()` - URL shortener helper

### System Utilities (`utils/system_utils.py`)
- `get_disk_usage()` - Get disk space info
- `get_system_info()` - Get OS and hardware info
- `find_large_files()` - Find large files in directory
- `monitor_process()` - Monitor process resource usage

## Quick Start

```python
from utils.file_utils import find_files, get_file_info
from utils.text_utils import extract_emails, slugify
from utils.date_utils import time_ago

# Find all Python files
python_files = find_files(".", "*.py")

# Extract emails from text
emails = extract_emails("Contact us at hello@example.com")

# Get human-readable time
print(time_ago(datetime(2024, 1, 1)))  # "11 months ago"
```

## Contributing

This project grows with daily contributions! Here are areas you can improve:

### Ideas for Daily Commits
1. **Add new utility functions** - Think of common tasks you do repeatedly
2. **Improve existing functions** - Add error handling, edge cases
3. **Add unit tests** - Increase test coverage
4. **Add documentation** - Improve docstrings and examples
5. **Performance optimizations** - Make functions faster
6. **Add CLI support** - Make utilities runnable from command line
7. **Add type hints** - Improve code quality
8. **Fix bugs** - Address edge cases and issues

### Contribution Areas
- [ ] Add JSON/CSV/XML parsing utilities
- [ ] Add image processing utilities
- [ ] Add encryption/hashing utilities
- [ ] Add logging utilities
- [ ] Add configuration management
- [ ] Add database utilities
- [ ] Add email sending utilities
- [ ] Add PDF utilities
- [ ] Add archive (zip/tar) utilities
- [ ] Add network utilities

## Next Challenge

### 🚀 Your Next Coding Challenge

Now that you've built a comprehensive Python utils toolkit, here's your next challenge:

**Build a CLI Tool for the Utils Toolkit**

Create a command-line interface that allows users to access all utility functions from the terminal. This will make your utilities more accessible and demonstrate advanced CLI development skills.

**Requirements:**
- Use `argparse` or `click` for CLI parsing
- Support all major utility functions (file, text, date, web, system)
- Include help documentation for each command
- Add progress bars for long-running operations
- Support both interactive and batch modes
- Include configuration file support
- Add colored output for better user experience

**Example Usage:**
```bash
# File operations
python -m utils.cli find-files --pattern "*.py" --directory ./src
python -m utils.cli organize-files --source ./downloads --by extension

# Text processing
python -m utils.cli extract-emails --file document.txt
python -m utils.cli slugify "Hello World! How are you?"

# System info
python -m utils.cli system-info
python -m utils.cli disk-usage C:/
```

**Bonus Challenges:**
- Add shell completion support (bash/zsh/fish)
- Create a web API version of the utilities
- Add logging and audit trails
- Implement plugin architecture for extensibility
- Create a GUI version using tkinter or web interface

**Learning Objectives:**
- CLI application development
- Argument parsing and validation
- Cross-platform compatibility
- Error handling and user feedback
- Code organization for CLI tools

---

## License

MIT License - Feel free to use, modify, and distribute.

## Author

Your Name

---

*This toolkit is designed to be a living project with continuous improvements. Star the repo and check back for updates!*
