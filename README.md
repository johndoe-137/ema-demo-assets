# Ema - Procure-to-Pay Demo Assets

This repository contains the sample data files used for the **Ema Procure-to-Pay AI Employee** live prototype. It acts as a persistent, version-controlled "simulated data lake" for the demonstration.

The main prototype, located at [johndoe-137/ema_prototype_demo](https://github.com/johndoe-137/ema_prototype_demo), automatically clones this repository to ingest these files during the live demo.

---
## Contents

All demo files are located within the `/simulated_data_lake/` directory. The files are a mix of PDFs and images (`.png`, `.jpg`) to simulate the chaotic, multi-format nature of a real-world data lake.

The documents are organized into three distinct business scenarios designed to test the AI's capabilities.

### Document Scenarios

| Filename | Format | Scenario | Purpose |
| :--- | :--- | :--- | :--- |
| `PO-101.pdf` | PDF | 1: Happy Path | The baseline purchase order. |
| `INV-CD-101.pdf` | PDF | 1: Happy Path | The corresponding invoice that perfectly matches the PO. |
| `GRN-101.png` | Image | 1: Happy Path | A high-quality scan of the Goods Received Note. |
| `PO-102.pdf` | PDF | 2: Exception Path | A standard purchase order. |
| `INV-RS-102.pdf` | PDF | 2: Exception Path | The invoice containing a deliberate **quantity mismatch** and financial errors. |
| `GRN-102.jpg` | Image | 2: Exception Path | A lower-quality scan of the GRN to test OCR robustness. |
| `PO-103.pdf` | PDF | 3: Fuzzy Match | A PO with a specific, hyphenated item description. |
| `INV-TD-103.pdf` | PDF | 3: Fuzzy Match | The invoice with a **semantically similar**, but not identical, item description. |

---
## Usage

This repository is intended to be used as a data source for the main interactive demo. The prototype in the primary project repository will automatically clone these assets into its environment upon execution. No manual download is required.
