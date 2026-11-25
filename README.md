# Medea — Medical Imaging & Dicom Viewer Suite

Medea is an offline-first DICOM medical imaging viewer, 3D volume reconstructor, and radiology workstation for Android and Desktop (Qt 6 with a **Vulkan 1.3 and DirectX 12 (Feature Level 12_1) First/Only** graphics rendering architecture). Built with C++20, Qt 6 / QML, and native ITK/VTK imaging libraries, Medea enables healthcare professionals and researchers to inspect MRI, CT, and X-ray DICOM datasets with zero cloud uploads or telemetry.

---

## ⚡ Core Subsystems & Status Matrix

| Subsystem | Features & Capabilities | Status / Roadmap |
|---|---|---|
| **Graphics Engine** | **Vulkan 1.3 & DirectX 12 (Feature Level 12_1) First/Only** desktop viewport | Active |
| **DICOM Inspector** | DICOM file parsing, window/level adjustments, Multi-Planar Reconstruction (MPR) | Active |
| **3D Volume Renderer** | Cinematic 3D volume rendering, ISO-surface extraction, anisotropic diffusion filter | Roadmap |
| **PACS Integration** | Local DICOM PACS server client (C-STORE / C-FIND / C-MOVE) | Roadmap |
| **Measurement Suite** | Hounsfield Unit (HU) ROI density measurements, calipers, text annotations | Active |
| **AI Segmentation** | Automatic organ segmentation, bone suppression filter, anonymized DICOM exporter | Roadmap |

---

## 🩺 Key Features & Subsystem Breakdown

### 🩻 DICOM Viewing & Multi-Planar Reconstruction (`dicom`)
- **Current**: DICOM file parsing, window/level (brightness/contrast) adjustment, Multi-Planar Reconstruction (MPR: Axial, Sagittal, Coronal cuts), and measurement tools (length, angle, HU density).
- **Planned / Roadmap**: Cinematic 3D volume rendering, ISO-surface extraction, anisotropic diffusion filtering, and DICOM PACS server connection (C-STORE / C-FIND).

### 📐 Measurement & Annotation Suite (`tools`)
- **Current**: Hounsfield Unit (HU) region-of-interest (ROI) measurements, caliper tools, text annotations, and keyframe export.
- **Planned / Roadmap**: Automatic organ segmentation, bone suppression filter, and anonymized DICOM exporter.

---

## 🏗️ Architecture & Technology Stack

- **Graphics APIs**: Vulkan 1.3 & DirectX 12 (Feature Level 12_1) First/Only.
- **UI Shell**: Qt 6.12 / QML for Desktop, Jetpack Compose for Android.
- **Image Core**: C++20, DCMTK (DICOM Toolkit), VTK (Visualization Toolkit) rendering core.
- **Licensing**: AGPL-3.0.

---

## 🛠️ Building & Running

### Desktop
```bat
build.bat Release
run.bat
```

---

## 📜 License

Medea is released under the **GNU Affero General Public License v3.0** (AGPL-3.0). See [`LICENSE`](LICENSE) for details.
