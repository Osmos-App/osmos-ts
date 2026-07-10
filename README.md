# Osmos Desktop Client (`osmos-ts`)

A cross-platform desktop application for the **[Osmos](https://useosmos.com)** local-first version control system, built with **Tauri**, **React**, and **TypeScript**. 

This app provides a premium, user-friendly graphical interface for managing repositories, tracking working-tree changes, committing snapshots, switching branches, and merging conflicts across Windows, macOS, and Linux.

## Architecture

This frontend client interacts with the `osmos-core` daemon:

- **Frontend:** React + TypeScript (Vite)
- **Backend:** Tauri (Rust)
- **Core:** The `osmos-core` daemon running locally, handling all file hashing, encryption, and peer-to-peer sync via mDNS.

## Development Setup

### Prerequisites
- Node.js & npm
- Rust (for Tauri backend)
- OS-specific dependencies for Tauri (e.g., `webkit2gtk` on Linux, Xcode on macOS, Visual Studio C++ on Windows)

### Running Locally

1. Install dependencies:
   ```bash
   npm install
   ```

2. Start the development server:
   ```bash
   npm run tauri dev
   ```
