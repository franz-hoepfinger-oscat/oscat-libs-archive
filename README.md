# OSCAT Libraries Legacy Archive

⚠️ **ARCHIVED REPOSITORY**  
This repository is an archive containing historical, legacy versions of the OSCAT (Open Source Community for Automation Technology) libraries. It is marked as archived and read-only, meaning it is no longer actively maintained, and no further updates or contributions will be accepted.

---

## Overview

OSCAT provides open-source libraries for PLC programming according to the IEC 61131-3 standard. These libraries are designed to be hardware-independent and highly portable across various PLC platforms (such as CoDeSys 2.x, CoDeSys 3.x, TwinCAT, Step 7, PCWorx, etc.).

This repository preserves the historical artifacts and releases of the three main OSCAT libraries:
*   **OSCAT BASIC:** The foundation library containing mathematical functions, string helpers, date/time tools, control loops, and more.
*   **OSCAT BUILDING:** Specialized functions for building automation and HVAC applications.
*   **OSCAT NETWORK:** Functions for networking protocols and communication.

For details on the project's background, see the [OSCAT Overview](OSCAT overview.md) (or the original [OSCAT overview.pdf](OSCAT overview.pdf)).

---

## Repository Structure

The archive is organized by library:

*   **[OSCAT BASIC](OSCAT_BASIC_LIB/)**
    *   [License Agreement](OSCAT_BASIC_LIB/License%20Agreement.md) ([Original PDF](OSCAT_BASIC_LIB/License%20Agreement.pdf))
    *   **[ARCHIVE/](OSCAT_BASIC_LIB/ARCHIVE/)**: Historical releases (from version 1.10 up to 3.36), each including the library files (`.lib`, `.exp`), revision history (`.md`, `.pdf`, `.ods`), and documentation.
*   **[OSCAT BUILDING](OSCAT_BUILDING_LIB/)**
    *   [License Agreement](OSCAT_BUILDING_LIB/License%20Agreement.md) ([Original PDF](OSCAT_BUILDING_LIB/License%20Agreement.pdf))
    *   **[Archive/](OSCAT_BUILDING_LIB/Archive/)**: Historical releases (version 1.00).
*   **[OSCAT NETWORK](OSCAT_NETWORK_LIB/)**
    *   [License Agreement](OSCAT_NETWORK_LIB/License%20Agreement.md) ([Original PDF](OSCAT_NETWORK_LIB/License%20Agreement.pdf))
    *   **[Archive/](OSCAT_NETWORK_LIB/Archive/)**: Historical releases (from net100 to net135).

---

## Licenses

The OSCAT libraries are free of charge for both private and commercial usage. Each library has its own license agreement.

> [!IMPORTANT]
> While OSCAT now publishes its work under the Eclipse Public License 2.0 (EPL-2.0), the archived legacy files in this repository are **excluded** from the EPL-2.0 license. This is because these files were created and distributed prior to OSCAT's migration to the Eclipse Foundation. Instead, they remain governed by their original respective license agreements.

For a complete overview and links to all licenses, please see [LICENSE.md](LICENSE.md) in the root of this repository.

---

## Historical Releases & Downloads

> **Current Documentation:** https://oscat.readthedocs.io

### CODESYS V2.3

#### OSCAT Basic 3.36

- [Folder](https://github.com/eclipse-oscat/oscat-libs-archive/tree/main/OSCAT_BASIC_LIB/ARCHIVE/rel336)
- [oscat_basic_336.lib](https://github.com/eclipse-oscat/oscat-libs-archive/raw/refs/heads/main/OSCAT_BASIC_LIB/ARCHIVE/rel336/oscat_basic_336.lib)

#### OSCAT Network 1.21 HF1

- [Folder](https://github.com/eclipse-oscat/oscat-libs-archive/tree/main/OSCAT_NETWORK_LIB/Archive/net121)
- [codesys_network_121_hf1.lib](https://github.com/eclipse-oscat/oscat-libs-archive/raw/refs/heads/main/OSCAT_NETWORK_LIB/Archive/net121/codesys_network_121_hf1.lib)
- [Docs (DE)](https://github.com/eclipse-oscat/oscat-libs-archive/raw/refs/heads/main/OSCAT_NETWORK_LIB/Archive/net121/oscat_netlib121_de.pdf)
- [Docs (EN)](https://github.com/eclipse-oscat/oscat-libs-archive/raw/refs/heads/main/OSCAT_NETWORK_LIB/Archive/net121/oscat_netlib121_en.pdf)

#### OSCAT Network 1.35

- [Folder](https://github.com/eclipse-oscat/oscat-libs-archive/tree/main/OSCAT_NETWORK_LIB/Archive/net135)
- [codesys_network_135.lib](https://github.com/eclipse-oscat/oscat-libs-archive/raw/refs/heads/main/OSCAT_NETWORK_LIB/Archive/net135/codesys_network_135.lib)
- [Docs (DE)](https://github.com/eclipse-oscat/oscat-libs-archive/raw/refs/heads/main/OSCAT_NETWORK_LIB/Archive/net135/oscat_netlib135_de.pdf)

#### OSCAT Building 1.00

- [Folder](https://github.com/eclipse-oscat/oscat-libs-archive/tree/main/OSCAT_BUILDING_LIB/Archive/rel100)
- [oscat_building_100.lib](https://github.com/eclipse-oscat/oscat-libs-archive/raw/refs/heads/main/OSCAT_BUILDING_LIB/Archive/rel100/oscat_building_100.lib)
- [Docs (DE)](https://github.com/eclipse-oscat/oscat-libs-archive/raw/refs/heads/main/OSCAT_BUILDING_LIB/Archive/rel100/oscat_building100_de.pdf)
- [Docs (EN)](https://github.com/eclipse-oscat/oscat-libs-archive/raw/refs/heads/main/OSCAT_BUILDING_LIB/Archive/rel100/oscat_building100_en.pdf)

### CODESYS V3

#### OSCAT Basic 3.35

- [Folder](https://github.com/eclipse-oscat/oscat-libs-archive/tree/main/OSCAT_BASIC_LIB/ARCHIVE/rel335)
- [oscat_basic_335.library](https://github.com/eclipse-oscat/oscat-libs-archive/raw/refs/heads/main/OSCAT_BASIC_LIB/ARCHIVE/rel335/oscat_basic_335.library)

#### OSCAT Network 1.35

Please use the V2.3 version, there is no explicit port for V3.

- [Folder](https://github.com/eclipse-oscat/oscat-libs-archive/tree/main/OSCAT_NETWORK_LIB/Archive/net135)
- [Docs (DE)](https://github.com/eclipse-oscat/oscat-libs-archive/raw/refs/heads/main/OSCAT_NETWORK_LIB/Archive/net135/oscat_netlib135_de.pdf)

#### OSCAT Building 1.00

- [Folder](https://github.com/eclipse-oscat/oscat-libs-archive/tree/main/OSCAT_BUILDING_LIB/Archive/rel100)
- [oscat_building_100.lib](https://github.com/eclipse-oscat/oscat-libs-archive/raw/refs/heads/main/OSCAT_BUILDING_LIB/Archive/rel100/oscat_building_100.lib)
- [Docs (DE)](https://github.com/eclipse-oscat/oscat-libs-archive/raw/refs/heads/main/OSCAT_BUILDING_LIB/Archive/rel100/oscat_building100_de.pdf)
- [Docs (EN)](https://github.com/eclipse-oscat/oscat-libs-archive/raw/refs/heads/main/OSCAT_BUILDING_LIB/Archive/rel100/oscat_building100_en.pdf)

### Beckhoff

#### OSCAT Network 1.21

- [Folder](https://github.com/eclipse-oscat/oscat-libs-archive/tree/main/OSCAT_NETWORK_LIB/Archive/net121)
- [beckhoff_network_121.lib](https://github.com/eclipse-oscat/oscat-libs-archive/raw/refs/heads/main/OSCAT_NETWORK_LIB/Archive/net121/beckhoff_network_121.lib)
- [Docs (DE)](https://github.com/eclipse-oscat/oscat-libs-archive/raw/refs/heads/main/OSCAT_NETWORK_LIB/Archive/net121/oscat_netlib121_de.pdf)
- [Docs (EN)](https://github.com/eclipse-oscat/oscat-libs-archive/raw/refs/heads/main/OSCAT_NETWORK_LIB/Archive/net121/oscat_netlib121_en.pdf)

### Siemens S7

#### OSCAT Basic 3.32

- [Folder](https://github.com/eclipse-oscat/oscat-libs-archive/tree/main/OSCAT_BASIC_LIB/ARCHIVE/rel332)
- [oscat_basic_332_s7.zip](https://github.com/eclipse-oscat/oscat-libs-archive/raw/refs/heads/main/OSCAT_BASIC_LIB/ARCHIVE/rel332/oscat_basic_332_s7.zip)

#### OSCAT Network

Not available

#### OSCAT Building 1.00

- [Folder](https://github.com/eclipse-oscat/oscat-libs-archive/tree/main/OSCAT_BUILDING_LIB/Archive/rel100)
- [s7_building_100.zip](https://github.com/eclipse-oscat/oscat-libs-archive/raw/refs/heads/main/OSCAT_BUILDING_LIB/Archive/rel100/s7_building_100.zip)
- [Docs (DE)](https://github.com/eclipse-oscat/oscat-libs-archive/raw/refs/heads/main/OSCAT_BUILDING_LIB/Archive/rel100/oscat_building100_de.pdf)
- [Docs (EN)](https://github.com/eclipse-oscat/oscat-libs-archive/raw/refs/heads/main/OSCAT_BUILDING_LIB/Archive/rel100/oscat_building100_en.pdf)

### PC Worx

#### OSCAT Basic 3.33

- [Folder](https://github.com/eclipse-oscat/oscat-libs-archive/tree/main/OSCAT_BASIC_LIB/ARCHIVE/rel333)
- [pcworx_basic_333.zip](https://github.com/eclipse-oscat/oscat-libs-archive/raw/refs/heads/main/OSCAT_BASIC_LIB/ARCHIVE/rel333/pcworx_basic_333.zip)
- [Docs (DE)](https://github.com/eclipse-oscat/oscat-libs-archive/raw/refs/heads/main/OSCAT_BASIC_LIB/ARCHIVE/rel333/oscat_basic333_de.pdf)
- [Docs (EN)](https://github.com/eclipse-oscat/oscat-libs-archive/raw/refs/heads/main/OSCAT_BASIC_LIB/ARCHIVE/rel333/oscat_basic333_en.pdf)

#### OSCAT Network 1.21

- [Folder](https://github.com/eclipse-oscat/oscat-libs-archive/tree/main/OSCAT_NETWORK_LIB/Archive/net121)
- [pcworx_network_121.zip](https://github.com/eclipse-oscat/oscat-libs-archive/raw/refs/heads/main/OSCAT_NETWORK_LIB/Archive/net121/pcworx_network_121.zip)
- [Docs (DE)](https://github.com/eclipse-oscat/oscat-libs-archive/raw/refs/heads/main/OSCAT_NETWORK_LIB/Archive/net121/oscat_netlib121_de.pdf)
- [Docs (EN)](https://github.com/eclipse-oscat/oscat-libs-archive/raw/refs/heads/main/OSCAT_NETWORK_LIB/Archive/net121/oscat_netlib121_en.pdf)

#### OSCAT Building 1.00

- [Folder](https://github.com/eclipse-oscat/oscat-libs-archive/tree/main/OSCAT_BUILDING_LIB/Archive/rel100)
- [pcworx_building_100_hotfix_1.zip](https://github.com/eclipse-oscat/oscat-libs-archive/raw/refs/heads/main/OSCAT_BUILDING_LIB/Archive/rel100/pcworx_building_100_hotfix_1.zip)
- [Docs (DE)](https://github.com/eclipse-oscat/oscat-libs-archive/raw/refs/heads/main/OSCAT_BUILDING_LIB/Archive/rel100/oscat_building100_de.pdf)
- [Docs (EN)](https://github.com/eclipse-oscat/oscat-libs-archive/raw/refs/heads/main/OSCAT_BUILDING_LIB/Archive/rel100/oscat_building100_en.pdf)




