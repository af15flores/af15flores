To install **Wine** on a Mac with an **M1 or M2 chip**, follow these steps:

### **Step 1: Install Homebrew**
If you haven’t already installed Homebrew, open **Terminal** and run:
```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
Once installed, update Homebrew:
```sh
brew update
```

### **Step 2: Install Rosetta 2 (if not installed)**
Rosetta 2 allows you to run x86 apps on Apple Silicon.
```sh
softwareupdate --install-rosetta --agree-to-license
```

### **Step 3: Install Wine**
Since Wine runs Windows applications, you need a version that supports **macOS ARM**. Use the following:
```sh
brew install --cask wine-stable
```
or, for a development version:
```sh
brew install --cask wine-devel
```

### **Step 4: Verify Installation**
Check if Wine is installed correctly:
```sh
wine --version
```

### **Step 5: Run Windows Applications**
1. Navigate to the `.exe` file directory:
   ```sh
   cd /path/to/windows_program/
   ```
2. Run the Windows program:
   ```sh
   wine program.exe
   ```

### **Alternative: Use Wine via UTM or Crossover**
- **[UTM](https://mac.getutm.app/)**: Emulates a full Windows environment.
- **[CrossOver](https://www.codeweavers.com/crossover)** (paid): Optimized Wine version for macOS ARM.

Would you like help setting up a specific Windows app on Wine?
