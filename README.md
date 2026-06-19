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

To provide a convenient landing page and download link for each major release, please refer to the [GitHub Releases page](https://github.com/franz-hoepfinger-oscat/oscat-libs-archive/releases). You can download specific legacy versions directly from there or explore the respective folders in the repository.