# Install Autopsy and Analyze the Disk File and Folder Configuration

## AIM
To install **Autopsy** and use it to analyze the disk’s file and folder configuration for forensic investigation.

## REQUIREMENTS
- **Operating System**: Windows 10/11, macOS, or Linux
- **Tools**:  
  - [Autopsy Digital Forensics Platform](https://www.autopsy.com/)  
  - Optional: Sleuth Kit CLI tools for deeper analysis
- **Test Data**: Disk image file (`.dd`, `.img`, `.E01`)

## ARCHITECTURE DIAGRAM
```mermaid
flowchart TD
    A[Disk Image / Physical Drive] --> B[Install Autopsy]
    B --> C[Create New Case in Autopsy]
    C --> D[Add Data Source: Disk Image]
    D --> E["Autopsy Modules Run: File System, Metadata, Keywords"]
    E --> F[File & Folder Structure View]
    F --> G[Export / Recover Files]
```
## DESIGN STEPS:
### Step 1:
Download Autopsy from the official website and install it on your system.

### Step 2:
Launch Autopsy and create a new case.

### Step 3:
Add your disk image or physical drive as the data source.

### Step 4:
Allow Autopsy to run its built-in ingest modules (file system analysis, hash lookup, keyword search, metadata extraction).

### Step 5:
View the file and folder hierarchy in the left-hand tree panel.

### Step 6:
Export or recover files if required for the investigation.

## PROGRAM(Windows)

1. Download Autopsy from autopsy.com.
2. Install and launch the application.
3. Select **New Case → Name your case → Choose case folder**.
4. Click Add **Data Source → Select Disk Image → Browse to file**.
5. Choose ingest modules (file system, metadata, hash lookup, keyword search).
6. Wait for processing to finish.
7. Explore file/folder structure in the navigation pane.
8.Export selected files for further examination.

## OUTPUT:
File and Folder Configuration Analysis Results
<img width="1132" height="597" alt="Screenshot 2026-11-02 105711" src="https://github.com/user-attachments/assets/0caefc57-d2b9-47fc-83ab-3bb382b92a3a" />

<img width="1145" height="597" alt="Screenshot 2026-11-02 105729" src="https://github.com/user-attachments/assets/086dcc35-71bf-4285-9e3f-f7f9d40e1407" />

<img width="1143" height="572" alt="Screenshot 2026-11-02 105757" src="https://github.com/user-attachments/assets/aeac4647-ce10-4392-8b3b-1f6a2ebb0a4a" />

<img width="1136" height="595" alt="Screenshot 2026-11-02 105821" src="https://github.com/user-attachments/assets/4de3d32e-3a94-4b71-b127-eadbb0c11cd4" />



## RESULT:
Autopsy was installed successfully and used to analyze disk, file, and folder configuration for forensic investigation.
