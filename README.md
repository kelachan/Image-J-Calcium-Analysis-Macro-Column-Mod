# Image-J-Calcium-Analysis-Macro-Column-Mod
Modified ImageJ calcium analysis macro to accommodate column scaling. Image preprocessing, cell segmentation into ROIs, application of different intensity thresholds, and .xlsx results included. Distance from column center and distance from column edge added to results in addition to standard intensity calculations.

**Required Fiji Plugins**

Before running the macro, ensure the following plugins are installed and up to date:
1. Trainable Weka Segmentation - Pre-installed in Fiji
2. Noise2Void (N2V) - Optional preprocessing step, denoising using deep learning
3. Template Matching - Optional preprocessing step, slice alignment

Go to Help → Update... Click Manage Update Sites, and enable CSBDeep and Template_Matching. Then,  Apply Changes, and restart Fiji.



**Use of Macro**

1. Download the macro file, F_Fo_macro_combined.ijm from this repository.
2. Open Fiji, then go to: Plugins → Macros → Run… and select the macro file.
3. Select the image to run the analysis on. 
4. Follow the on-screen dialogs.

You can try the macro using the sample time-lapse .czi image provided here: https://drive.google.com/drive/u/2/folders/12Kj8ol_rpForezNu8eSBeFmZKQFcjKAJ


When working in Windows, users should avoid using system-protected directories such as C:\Users, C:\Program Files, or the Fiji installation directory for storing input or output data. It is recommended to use an external folder to avoid write permission errors. All analysis outputs - ROI ZIP files for reference, a ΔF/F₀ CSV table, and graph images - are saved automatically to the same directory as the input image file.


