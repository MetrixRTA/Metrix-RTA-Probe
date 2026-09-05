# 🎧 Metrix RTA Probe

**Metrix RTA Probe** is a lightweight Windows utility for inspecting the real capabilities of **WASAPI** and **ASIO** audio devices.

## 📥 Download

### [⬇️ Download Metrix RTA Probe 0.1.0 x64](https://github.com/MetrixRTA/Metrix-RTA-Probe/releases/download/v0.1.0/MetrixRTAProbe_0.1.0_x64.exe)

> **Windows x64 only.** No installation is required.

## ✨ Features

- Detects active **Windows audio endpoints**
- Detects registered **64-bit ASIO drivers**
- Tests WASAPI devices in **Exclusive Mode**
- Opens and starts real native audio streams
- Checks sample rates from **8 kHz to 768 kHz**
- Tests **8-, 16-, 24- and 32-bit integer formats**
- Tests **32-bit floating-point formats**
- Checks **mono and multichannel configurations** separately
- Reports native **ASIO channel formats**
- Organizes supported frequencies by **bit depth and channel count**
- Displays driver file, version, provider, INF package and PnP information
- Supports multiple independent probe windows
- Copies complete reports to the clipboard

## ⚙️ How It Works

### WASAPI

WASAPI endpoints are tested in **Exclusive Mode** through the native `IAudioClient` interface.

A format is reported only when the corresponding native stream can be:

1. Opened successfully
2. Initialized in Exclusive Mode
3. Started successfully

### ASIO

ASIO drivers are accessed directly through their native **64-bit `IASIO` interface**.

The application verifies:

- Native channel formats
- Available input and output channels
- Supported sample rates
- Buffer creation
- ASIO engine startup

## 🖥️ System Requirements

- **Windows 10 or Windows 11**
- **64-bit operating system**
- A WASAPI-compatible audio device or registered 64-bit ASIO driver

## 🚀 Usage

1. Launch `MetrixRTAProbe_0.1.0_x64.exe`
2. Double-click a WASAPI endpoint or ASIO driver
3. Wait for the progress indicator to complete
4. Review the supported formats and driver information
5. Click **Copy** to copy the complete report
6. Click **Close** to close the report window

## ☕ Support

If you find this utility useful, you can support the project on **ko-fi**:

### [Support Metrix RTA on ko-fi](https://ko-fi.com/metrixrta)

<img width="120" height="120" alt="image" src="https://github.com/user-attachments/assets/862dc674-2e05-4170-bbf9-49cfc93d828d" />

