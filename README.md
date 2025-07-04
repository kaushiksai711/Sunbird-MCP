# Sunbird Content Search MCP Server

A Model Context Protocol (MCP) server for searching and accessing educational content from Sunbird, an open-source digital infrastructure for education.

## 🌟 Overview

The Sunbird Content Search MCP Server provides search and content retrieval capabilities for Sunbird's educational resources. This server implements the Model Context Protocol (MCP) standard to enable integration with educational platforms.

## 🎯 Key Features

### 🔍 Search Functionality
- Search across multiple content categories (Digital Textbook, Course, etc.)
- Filter by educational board (CBSE, State boards)
- Grade level filtering (Class 1-12)
- Language support (English, Hindi)
- Subject and audience type filtering

### 📚 Content Access
- Retrieve educational materials by content ID
- Stream PDF content directly
- Filter out ECML content for cleaner results
- Currently supports PDF format

## 🚀 Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/sunbird-ed/sunbird-mcp.git
   cd sunbird-mcp/sunbird_mcp
   ```

2. **Set up the environment**
   ```bash
   # Using uv (recommended)
   uv venv
   
   # Or using venv
   python -m venv .venv
   source .venv/bin/activate  # On Windows: .venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   # Using uv
   uv pip install -r pyproject.toml --extra dev
   
   # Or using pip
   pip install -e .[dev]
   ```
    
4. **Start the server**
   Go to to sunbird_mcp/src and run the following
   ```bash
   python -m __init__ sse
   ```

## 🛠️ Development

### Directory Structure
```
sunbird_mcp/
├── .vscode/         # VSCode configuration
├── inspector/       # MCP Inspector files
├── src/             # Source code
│   ├── __init__.py  # Package initialization
│   └── server.py    # Main server implementation
├── .env.example     # Example environment variables
├── pyproject.toml   # Project dependencies
└── README.md        # Project documentation
```

## 🙏 Acknowledgments

- Sunbird Community
- MCP Community

---

Built for the Sunbird ecosystem
