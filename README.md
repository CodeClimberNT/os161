# OS/161 Laboratory

This repository is the result of laboratory work developed during the *Programmazione di Sistema* course at the **Politecnico di Torino**. It represents an evolving project aimed at understanding system programming concepts via OS/161, a simulated operating system.

## Overview

The project features:
- A build system based on BSD make (bmake) to compile the OS/161 system.
- A simulated environment using the sys161 simulator to run the kernel.
- Custom modifications and experiments carried out as part of the laboratory work.

## How to Build and Run

### Prerequisites

- **bmake**: Ensure that BSD make is installed.
- **sys161**: The simulator required to run the OS/161 kernel.
- A Linux environment configured for system programming.

### Building the System

1. Open a terminal and navigate to the OS/161 source directory:
   ```bash
   cd ~/os161/src
   ```
2. Execute the rebuild command:
   ```bash
   bmake rebuild
   ```
   This will clean and compile the entire system.

### Running the Kernel

Once the build completes, launch the sys161 simulator with the kernel image:

1. Navigate to the install directory:
   ```bash
   cd ~/os161/root
   ```
2. Start the simulator:
   ```bash
   sys161 kernel
   ```

Alternatively, you can use the Visual Studio Code launch configurations provided in the repository to build and run the system directly from the IDE.

> [!Warning]
> If you can see this warning is highly possible that I didn't fix the `launch.json` file to run the kernel from the ide. For now the preferred (and working) method is to run it directly from the shell.

## License

- **Original Code:** The original OS/161 code is distributed under its original BSD-style license as detailed in the included NOTICE file. All the conditions listed there must be preserved in redistributions.
- **Modifications & Additions:** All modifications, enhancements, and additional content in this repository are licensed under the **MIT License**.
  
This dual licensing approach ensures that while the core OS/161 system remains bound by its original terms, any new contributions made as part of this laboratory project are available under the more permissive MIT terms.

For full details, please refer to the [NOTICE](NOTICE) file for the original license and the [LICENSE](LICENSE) file for the MIT license.

---

*Developed as part of the Politecnico di Torino's "Programmazione di Sistema" course.*