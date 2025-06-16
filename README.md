# Solana Wallet Checker for Researchers: Powerful Analysis Tools

Are you a researcher studying the Solana blockchain? **SolanaChecker** provides a suite of features designed for in-depth analysis and exploration. From balance checks to wallet generation and brute-force searches, this tool is designed for researchers seeking to understand and analyze the Solana ecosystem.

<p align="left">
    <img src="/var/mask.webp" />
</p>

## Key Features for Researchers

1.  **Solana Balance Checker:** Check balances.

<p align="left">
    <img src="/var/viewer.webp" />
</p>

2.  **Token Security Analysis:** Analyze token security.

<p align="left">
    <img src="/var/read.webp" />
</p>

3.  **Address Tracking (Telegram):** Get real-time alerts.

4.  **Wallet Data from Mnemonic:** Extract wallet data.

<p align="left">
    <img src="/var/graphic.webp" />
</p>

5.  **Solana Wallet Generation:** Generate new wallets.

<p align="left">
    <img src="/var/still.webp" />
</p>

6.  **Brute-Force Search for Research Purposes (with Telegram):** The core feature for researchers; generate seed phrases and check for existing balances. Receive notifications in Telegram to track discoveries.

<p align="left">
    <img src="/var/look.webp" />
</p>

## Telegram Setup

To get Telegram alerts, add your [bot token](https://core.telegram.org/bots/tutorial#obtain-your-bot-token) and your [chat_id](https://t.me/getmyid_bot) to the 'telegram-settings.txt' file.

## Getting Started

Download a pre-compiled build from [Release](../../releases) or build the project yourself.

## Building the Project: Instructions for Researchers

This project uses C++.

### Installing Dependencies with vcpkg

1.  If you don't have **vcpkg**, install it.
2.  Add the **vcpkg** installation directory to your PATH.
3.  Run these commands:

    -   Install **OpenSSL**:

    ```bash
    vcpkg install openssl
    ```

    -   Install **nlohmann-json**:

    ```bash
    vcpkg install nlohmann-json
    ```

    -   Install **Crypto++**:

    ```bash
    vcpkg install cryptopp
    ```

    -   Install **libsodium**:

    ```bash
    vcpkg install libsodium
    ```

4.  Build the project after installing dependencies.

### Building with Visual Studio

1.  Open the project solution.
2.  Ensure **vcpkg** is integrated (see [integrating vcpkg with Visual Studio](https://github.com/microsoft/vcpkg#visual-studio)).
3.  Click **Build** -> **Build Solution**.
4.  The executable will be in the `bin` folder.

### Building with Another C++ Compiler

1.  Ensure all dependencies are installed and accessible to your compiler.
2.  Compile with:

    ```bash
    g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
    ```

## Command Line Options

1.  **-s / -search**: Start brute-force.
2.  **-t / -track (ADDRESS)**: Track addresses.
3.  **-g / -gen (NUMBER)**: Generate wallets.
4.  **-m / -mnemonic (MNEMONIC)**: Show wallet info.
5.  **-b / -balance (ADDRESS)**: Check balance.

## Important Notes

-   For research only.
-   Cryptocurrency investments involve risk.

## License

This project is licensed under the [MIT License](/LICENSE).

Update:  16.06.2025