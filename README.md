# extforge

# Snail-IDE GUI

scratch-gui modified for use in [TurboWarp](https://turbowarp.org) then modified for use in [PenguinMod](https://penguinmod.com) then modified for use in [Snail-IDE](https://js.org) 😀

## Setup

To run Snail-IDE on your computer, follow these installation steps:

### 1. Prerequisites (Node.js & nvm)
You will need Node.js version 16 managed via Node Version Manager (nvm):
```bash
nvm install 16
nvm use 16
```
*(Windows users: Please accept any UAC administrative prompts that appear)*

### 2. Package Manager Setup
You need `pnpm` to resolve dependencies correctly. Install it globally:
```bash
npm install -g pnpm
```

### 3. Clone & Install
Clone the repository and install the project dependencies using the required hoist flag:
```bash
git clone https://github.com/snail-ide/snail-ide.github.io
cd snail-ide.github.io
pnpm i --shamefully-hoist
```

### 4. Running the Development Server
Launch the local server using your preferred package manager:
```bash
pnpm start
# OR
npm start
# OR
yarn start
```

### 💡 Node 17+ Compatibility
If you prefer to use Node.js version 17 or higher instead of version 16, you must pass the OpenSSL legacy provider flag to prevent cryptographic build errors.

* **Linux / macOS / GitHub Codespaces:** Run this in your terminal before starting:
  ```bash
  export NODE_OPTIONS=--openssl-legacy-provider
  ```
* **Windows (Command Prompt):**
  ```cmd
  set NODE_OPTIONS=--openssl-legacy-provider
  ```
* **Windows (PowerShell):**
  ```powershell
  \$env:NODE_OPTIONS="--openssl-legacy-provider"
  ```

## License

TurboWarp's modifications to Scratch are licensed under the GNU General Public License v3.0. See LICENSE or https://gnu.org for details.

The following is the original license for scratch-gui, which we are required to retain. This is NOT the license of this project.
