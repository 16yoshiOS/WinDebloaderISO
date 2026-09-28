# WinDebloaterISO

An advanced, user-centric fork of the original **tiny11builder** project. **WinDebloaterISO** gives you complete control over your custom Windows 11 builds, shifting away from hardcoded automation to a fully tailored, flexible experience.

## Why WinDebloaterISO?

The original tiny11builder blindly strips down Windows components using a fixed, unchangeable script. This often leads to unexpected side effects—such as losing critical gaming features like the Xbox Gaming Overlay or keeping bloated tools you don't need. 

**WinDebloaterISO** resolves this by introducing interactive format selections and an editable target list, letting the developer decide exactly what stays and what goes.

---

## 🔄 Direct Comparison: WinDebloaterISO vs. Original tiny11builder

| Feature / Capability | Original tiny11builder | **WinDebloaterISO (This Fork)** |
| :--- | :--- | :--- |
| **Output Image Formats** | Hardcoded to standard `.wim` only. | **Flexible Choice:** Select **ESD** (maximum compression, smaller ISO) or **WIM** (faster build process). |
| **App Removal List** | Runs automated, blind removal based on the author's fixed configuration. | **Fully Customizable:** Modify your application list on the fly to control exactly what gets targeted. |
| **Essential Gaming Protection** | High risk of stripping necessary gaming frameworks automatically. | **Total Control:** Safely preserve crucial components like `XboxGamingOverlay` if you need them. |
| **Bloatware Management** | Cannot adjust the removal list to target new system components. | **Scalable Scope:** Easily extend or shrink the removal script up to 69 custom entries or more. |

---

## 🚀 Key Advantages

* **Smart ESD Architecture:** Opting for the ESD format allows your 6-core processors (such as the AMD Ryzen 5 7430U) to leverage multithreaded compression, significantly driving down the final ISO footprint to around **5.57 GB** compared to bloated 8 GB retail files.
* **Component Granularity:** Eliminates the frustration of unexpected component stripping. Keep default system tools like the Windows Store, Paint, and Terminal while wiping out unwanted consumer bloatware.
* **Safety & Modification Safety:** Built directly on official DISM automation layers to prevent servicing stack corruption while maintaining image integrity.

## 🗺️ Roadmap / Future Plans

We aim to expand **WinDebloaterISO** into a deep OS optimization framework. Planned features for future releases include:

* **WinRE Removal Support:** Implementation of safe `winre.wim` target stripping to shrink the image footprint even further for ultra-lightweight installations.
* **SvcHost Optimization Layer:** Adding automated registry injection to modify `SvcHostSplitThresholdInKB` using precise decimal values, preventing unnecessary RAM splitting on systems with higher memory capacities.
* **Advanced Service Management:** Integrated scripts to completely disable, remove, or modify deep Windows system services on the fly during the offline image mounting phase.
