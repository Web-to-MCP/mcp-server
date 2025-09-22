# mcp-server# Web to MCP

**Send any website component to Cursor, Claude Code, or your AI coding assistant in one click.**

Web to MCP is a powerful browser extension and web service that bridges the gap between design and code by allowing you to capture website components and send them directly to your AI coding assistant using the Model Context Protocol (MCP).

## 🌟 Features

- **🎯 One-Click Component Capture**: Select any website element and send it directly to your AI assistant
- **🔗 MCP Integration**: Works seamlessly with Cursor IDE and Claude Code via Model Context Protocol
- **🎨 Pixel-Perfect References**: Capture actual rendered components with their exact styling
- **⚡ Lightning Fast**: 10x faster than traditional methods of describing UI components
- **🔒 Secure**: Google OAuth authentication with secure MCP channels
- **🌐 Universal**: Works with any website and any component
- **💳 Flexible Pricing**: Free tier available with premium features

## 🚀 Quick Start

### Prerequisites

- Chrome browser (latest version)
- Google account for authentication
- Cursor IDE or Claude Code (for MCP integration)

### Installation

1. **Install the Chrome Extension**
   ```bash
   # Visit the Chrome Web Store
   https://chromewebstore.google.com/detail/web-to-mcp/hbnhkfkblpgjlfonnikijlofeiabolmi
   ```

2. **Sign in to your account**
   - Click the extension icon
   - Authenticate with your Google account
   - Get your unique MCP URL

3. **Configure MCP in your AI tool**
   - Follow the setup guides below for Cursor or Claude Code
   - Add your MCP URL to enable direct component transfer

## 🛠️ Setup Guides

### For Cursor IDE

1. **Install the Chrome Extension** (see above)

2. **Configure MCP in Cursor**
   - Open Cursor Settings (`Ctrl+Shift+J` or `Cmd+Shift+J`)
   - Navigate to Features → Model Context Protocol
   - Create a new MCP configuration file

3. **Add MCP Configuration**
   Create `.cursor/mcp.json` in your project root:
   ```json
   {
     "mcpServers": {
       "web-to-mcp": {
         "url": "https://web-to-mcp.com/mcp/<YOUR_UNIQUE_ID>"
       }
     }
   }
   ```

4. **Start Capturing**
   - Navigate to any website
   - Click the extension icon
   - Select any component you want to capture
   - Reference it in Cursor using the component ID

### For Claude Code

1. **Install the Chrome Extension** (see above)

2. **Install Claude Code**
   ```bash
   # Download from https://claude.ai/code
   # Verify installation
   claude --version
   ```

3. **Add MCP Server**
   ```bash
   claude mcp add --transport http web-to-mcp https://web-to-mcp.com/mcp/<YOUR_UNIQUE_ID>
   ```

4. **Start Capturing**
   - Navigate to any website
   - Click the extension icon
   - Select any component you want to capture
   - Reference it in Claude Code using the component ID
