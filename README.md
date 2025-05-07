# Multi-Tab Browser Application

## Overview
This program creates a modern, multi-tab web browser using PyQt5 and QtWebEngine. It provides a clean and intuitive interface with essential browsing features.

## Key Features

### 1. Multi-Tab Support
- Create multiple browsing tabs
- Close tabs individually
- Always maintains at least one open tab
- Tab titles update to reflect webpage titles

### 2. Navigation System
- URL/Search bar that supports:
  - Direct URL navigation (e.g., `https://example.com`)
  - DuckDuckGo search integration for non-URL inputs
- Clean toolbar interface

### 3. User Interface
- Modern window layout
- Closable tabs
- URL bar with search functionality
- New Tab button in the toolbar

## Technical Implementation

### Main Components
- `SimpleBrowser`: Main window class inheriting from `QMainWindow`
- `QWebEngineView`: Powers the web rendering
- `QTabWidget`: Manages multiple browser tabs
- `QToolBar`: Contains navigation controls

### Key Methods
- `add_new_tab()`: Creates new browser tabs
- `navigate_to_url()`: Handles URL navigation and search
- `close_tab()`: Manages tab closure
- `update_urlbar()`: Keeps URL bar synchronized

## Requirements
```python
from PyQt5.QtWidgets import QApplication, QMainWindow, QToolBar, QLineEdit, QTabWidget
from PyQt5.QtWebEngineWidgets import QWebEngineView
from PyQt5.QtCore import QUrl
```

## Usage
To run the browser:
```bash
python browser_lab1.py
```

The browser will launch with a clean interface, ready for web browsing or searching via DuckDuckGo.
