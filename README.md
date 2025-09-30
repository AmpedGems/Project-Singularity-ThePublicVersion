PHASE 1 TAB - ALL ELEMENTS

1. (Button)
Name: "Browse / Drop Game file "APK-XAPK-APKS-APKM-ZIP""
Location: Docked at top of tab
Actions:
Click: Opens file dialog to browse and select game files (APK, XAPK, APKS, APKM, ZIP)
Drag Enter: Validates dragged files, shows copy cursor for valid game file types
Drag Drop: Processes dropped game files
What It Does: Allows users to select or drag-drop game files for processing. Validates AmpedGems location is set before proceeding. Resets text boxes and processes the selected file.

Example Running: 
[12:48:45] 🔄 Reset Phase 1 text boxes for new file selection
[12:48:45] 🚀 Starting game file selection...
[12:48:45] ========================================
[12:48:47] ❌ No file selected - workspace preserved
[12:48:47] ========================================
[12:48:47] ✅ Game file selection completed!

Example Running: 
[12:48:55] 🔄 Reset Phase 1 text boxes for new file selection
[12:48:55] 🚀 Starting game file selection...
[12:48:55] ========================================
[12:48:58] 📁 Selected file: GO+Hero+GO_42.0.0_apkcombo.com.xapk
[12:48:58] 🗂️ Clearing workspace...
[12:48:59] 📋 Copying file to workspace...
[12:49:01] ✅ File copied successfully: GO+Hero+GO_42.0.0_apkcombo.com.xapk -> a.xapk
[12:49:01] 🔓 Inject Empty Menu button re-enabled for new game file
[12:49:01] ========================================
[12:49:01] ✅ Game file selection completed!


2. (Label)
Name: "No File Selected" (default text)
Location: Below Button "Browse / Drop Game file "APK-XAPK-APKS-APKM-ZIP""
Actions: (display only)
What It Does: Displays the name of the currently selected game file


3. (Button)
Name: "Process Game File" 
Location: Below Label "No File Selected"
Actions:
Click: Runs complete 3-phase workflow to prepare game file
Drag Enter: Validates dragged game files
Drag Drop: Processes dropped game files directly
What It Does: Executes multi-step processing: converts to APK if needed, decompiles APK, and extracts metadata and creates marker files

Example Running: 
[12:54:46] 🔄 Reset Phase 1 text boxes for new file selection
[12:54:46] 🚀 Starting Multi-Step Game File Processing...
[12:54:46] ========================================
[12:54:46] 📋 Starting multi-step process...
[12:54:46] 🔄 This process includes multiple phases:
[12:54:46]    📦 Phase 1: APK Conversion (Split APK merging if needed)
[12:54:46]    🔧 Phase 2: APK Decompilation (Future implementation)
[12:54:46]    🎯 Phase 3: Game Analysis (Future implementation)
[12:54:46] 
[12:54:46] 🔄 === PHASE 1: APK CONVERSION ===
[12:54:46] 🔍 Detecting AmpedGems structure...
[12:54:46] 📁 Detected structure: New (tools folder)
[12:54:46] 🔍 Searching for APK file (a.*)...
[12:54:46] 📱 Found file: a.xapk
[12:54:46] 📦 Split APK format detected (.xapk), merging required...
[12:54:46] 📦 Extracting split APK archive...
[12:54:46] 🔍 Found 2 APK files in archive
[12:54:46] 🎯 Found main APK: com.PuzzlePoint.IdleRPG.apk
[12:54:46] 🔄 Merging...
[12:54:47] ✅ Merge completed successfully
[12:54:47] ✅ Split APK merged successfully: a_merged.apk
[12:54:48] 🧹 Starting cleanup process...
[12:54:48] 🗑️ Removing original split APK: a.xapk
[12:54:48] ✅ Original file removed successfully
[12:54:48] 📝 Renaming merged APK to standard name...
[12:54:48]    From: a_merged.apk
[12:54:48]    To: a.apk
[12:54:48] ✅ APK renamed successfully to: a.apk
[12:54:48] ✅ Cleanup completed. Final APK: a.apk
[12:54:48] 🎯 Final processed APK: a.apk
[12:54:48] 📋 APK conversion completed. Ready for next steps.
[12:54:48] ✅ Phase 1 completed successfully!
[12:54:48] 🔄 === PHASE 2: APK METADATA EXTRACTION ===
[12:54:48] 🔍 Detecting AmpedGems structure...
[12:54:48] 📁 Detected structure: New (tools folder)
[12:54:48] 🔍 Searching for APK file (a.apk)...
[12:54:48] 📱 Found APK: a.apk
[12:54:48] 📊 Extracting APK metadata and creating marker files...
[12:54:48] 📊 APK Metadata Extraction:
[12:54:48] ===========================
[12:54:48] 📤 package: name='com.PuzzlePoint.IdleRPG' versionCode='42' versionName='42.0.0'
[12:54:48] 📤 launchable-activity: name='com.unity3d.player.UnityPlayerActivity'
[12:54:48] 🔚 Process exit code: 0
[12:54:48] ✅ Package Name: com.PuzzlePoint.IdleRPG
[12:54:48] ✅ App Name: Go_Hero_Go
[12:54:48] ✅ Version: 42.0.0 (Code: 42)
[12:54:48] ✅ Launch Activity: com.unity3d.player.UnityPlayerActivity
[12:54:48] 📝 Updated Phase 1 text boxes with extracted metadata
[12:54:48] 📝 Creating marker files...
[12:54:48]    📄 Created: com.PuzzlePoint.IdleRPG.cpp
[12:54:48]    📄 Created: com.unity3d.player.UnityPlayerActivity.bitch
[12:54:48]    📄 Created: 42.0.0.version
[12:54:48]    📄 Created: Go_Hero_Go.name
[12:54:48] ✅ Created 4 marker files
[12:54:48] 📁 Renaming APK file...
[12:54:48] ✅ APK renamed to: com.PuzzlePoint.IdleRPG.apk
[12:54:48] ===========================
[12:54:48] 🎯 Metadata extraction and marker creation completed!
[12:54:48] 📋 APK metadata extraction and marker file creation completed!
[12:54:48] ✅ Phase 2 completed successfully!
[12:54:48] 🔄 === PHASE 3: APK DECOMPILATION ===
[12:54:48] 🔍 Detecting AmpedGems structure...
[12:54:48] 📁 Detected structure: New (tools folder)
[12:54:48] 🔍 Looking for .cpp marker files...
[12:54:48] 📦 Package name from marker: com.PuzzlePoint.IdleRPG
[12:54:48] ✅ Found corresponding APK: com.PuzzlePoint.IdleRPG.apk
[12:54:48] 📱 Using APK for decompilation: com.PuzzlePoint.IdleRPG.apk
[12:54:48] ⚙️ Do not decode sources: ✅ Enabled (faster, no smali)
[12:54:48] 🔧 Starting APK decompilation with APKTool...
[12:54:48] 📤 I: Using Apktool 2.11.0 on com.PuzzlePoint.IdleRPG.apk with 8 threads
[12:54:48] 📤 I: Copying raw classes.dex file...
[12:54:48] 📤 I: Copying raw classes2.dex file...
[12:54:48] 📤 I: Loading resource table...
[12:54:48] 📤 I: Decoding file-resources...
[12:54:48] 📤 I: Loading resource table from file: C:\Users\y\AppData\Local\apktool\framework\1.apk
[12:54:50] 📤 I: Decoding values */* XMLs...
[12:54:50] 📤 I: Decoding AndroidManifest.xml with resources...
[12:54:50] 📤 I: Regular manifest package...
[12:54:50] 📤 I: Copying original files...
[12:54:50] 📤 I: Copying assets...
[12:54:50] 📤 I: Copying lib...
[12:54:51] 📤 I: Copying kotlin...
[12:54:51] 📤 I: Copying unknown files...
[12:54:51] 🔚 Process exit code: 0
[12:54:51] ✅ APK decompilation completed successfully
[12:54:51] 📊 Decompilation Results:
[12:54:51] ========================
[12:54:51] ✅ AndroidManifest.xml - App configuration
[12:54:51] ✅ lib/ - Native libraries (1 architectures)
[12:54:51]    📱 arm64-v8a: 7 .so files
[12:54:51] ========================
[12:54:51] 🔧 Applying post-decompilation fixes...
[12:54:51] 🔧 Post-Decompilation Fixes:
[12:54:51] ==========================
[12:54:51]    ℹ️ AndroidManifest.xml already clean, no fixes needed
[12:54:51]    ℹ️ apktool.yml already configured correctly
[12:54:51]    ℹ️ Processed 10 files, no dummy entries found
[12:54:51] 🎯 Applied 0 post-decompilation fixes
[12:54:51] 💡 These fixes prepare the APK for successful recompilation
[12:54:51] ==========================
[12:54:51] 🎯 APK decompiled successfully to: com.PuzzlePoint.IdleRPG
[12:54:51] 📋 Metadata extraction, decompilation and post-processing completed. Files ready for analysis and recompilation.
[12:54:51] ✅ Phase 3 completed successfully!
[12:54:51] 🎯 Complete 3-phase APK processing completed successfully!
[12:54:51] ========================================
[12:54:51] ✅ Multi-step game file processing completed successfully!


4.  (Label)
Name: "Package Name:"
Actions:  (display label)
What It Does: Label for the package name text box

5.  (TextBox)
Properties: ReadOnly = true
Actions:  (display only)
What It Does: Displays the extracted package name from the processed game file


6.  (Label)
Name: "Game Name:"
Actions:  (display label)
What It Does: Label for the game name text box

7.  (TextBox)
Properties: ReadOnly = true
Actions:  (display only)
What It Does: Displays the extracted game name from the processed game file

8.  (Label)
Name: "Game Version:"
Actions:  (display label)
What It Does: Label for the game version text box

9.  (TextBox)
Properties: ReadOnly = true
Actions:  (display only)
What It Does: Displays the extracted game version from the processed game file

10.  (Label)
Name: "Build Number:"
Actions:  (display label)
What It Does: Label for the build number text box

11.  (TextBox)
Properties: ReadOnly = true
Actions:  (display only)
What It Does: Displays the extracted build number from the processed game file

12.  (Label)
Name: "Main Activity:"
Actions:  (display label)
What It Does: Label for the main activity text box

13.  (TextBox)
Properties: ReadOnly = true
Actions:  (display only)
What It Does: Displays the extracted main activity class from the processed game file

14.  (Button)
Name: "Convert To APK"
Location: Below metadata fields
Actions:
Click: Converts various game file formats (XAPK, APKS, APKM, ZIP) to standard APK format
What It Does: Processes and merges split APK files into a single standard APK file. Handles different game file formats and prepares them for decompilation.

Example Running: 
[13:21:09] 🔍 Detecting AmpedGems structure...
[13:21:09] 📁 Detected structure: New (tools folder)
[13:21:09] 🔍 Searching for APK file (a.*)...
[13:21:09] 📱 Found file: a.xapk
[13:21:09] 📦 Split APK format detected (.xapk), merging required...
[13:21:09] 📦 Extracting split APK archive...
[13:21:09] 🔍 Found 2 APK files in archive
[13:21:09] 🎯 Found main APK: com.PuzzlePoint.IdleRPG.apk
[13:21:09] 🔄 Merging...
[13:21:10] ✅ Merge completed successfully
[13:21:10] ✅ Split APK merged successfully: a_merged.apk
[13:21:10] 🧹 Starting cleanup process...
[13:21:10] 🗑️ Removing original split APK: a.xapk
[13:21:10] ✅ Original file removed successfully
[13:21:10] 📝 Renaming merged APK to standard name...
[13:21:10]    From: a_merged.apk
[13:21:10]    To: a.apk
[13:21:10] ✅ APK renamed successfully to: a.apk
[13:21:10] ✅ Cleanup completed. Final APK: a.apk
[13:21:10] 🎯 Final processed APK: a.apk
[13:21:10] 📋 APK conversion completed. Ready for next steps.
[13:21:10] ========================================
[13:21:10] ✅ APK conversion completed successfully!


15.  (Button)
Name: "Decompile"
Location: Next row
Actions:
Click: Decompiles APK files using APKTool
What It Does: Breaks down APK into readable files, extracts resources, code, and manifest files. Can skip source decoding based on checkbox setting.

Example Running: 
[13:23:23] 🚀 Starting APK Decompilation...
[13:23:23] ========================================
[13:23:23] 🔍 Detecting AmpedGems structure...
[13:23:23] 📁 Detected structure: New (tools folder)
[13:23:23] 🔍 Searching for APK file...
[13:23:23] 📱 Found APK: a.apk
[13:23:23] 📊 Extracting APK metadata and creating marker files...
[13:23:23] 📊 APK Metadata Extraction:
[13:23:23] ===========================
[13:23:23] 📤 package: name='com.PuzzlePoint.IdleRPG' versionCode='42' versionName='42.0.0'
[13:23:23] 📤 launchable-activity: name='com.unity3d.player.UnityPlayerActivity'
[13:23:23] 🔚 Process exit code: 0
[13:23:23] ✅ Package Name: com.PuzzlePoint.IdleRPG
[13:23:23] ✅ App Name: Go_Hero_Go
[13:23:23] ✅ Version: 42.0.0 (Code: 42)
[13:23:23] ✅ Launch Activity: com.unity3d.player.UnityPlayerActivity
[13:23:23] 📝 Updated Phase 1 text boxes with extracted metadata
[13:23:23] 📝 Creating marker files...
[13:23:23]    📄 Created: com.PuzzlePoint.IdleRPG.cpp
[13:23:23]    📄 Created: com.unity3d.player.UnityPlayerActivity.bitch
[13:23:23]    📄 Created: 42.0.0.version
[13:23:23]    📄 Created: Go_Hero_Go.name
[13:23:23] ✅ Created 4 marker files
[13:23:23] 📁 Renaming APK file...
[13:23:23] ✅ APK renamed to: com.PuzzlePoint.IdleRPG.apk
[13:23:23] ===========================
[13:23:23] 🎯 Metadata extraction and marker creation completed!
[13:23:23] 🔍 Locating renamed APK file based on .cpp marker...
[13:23:23] 🔍 Looking for .cpp marker files...
[13:23:23] 📦 Package name from marker: com.PuzzlePoint.IdleRPG
[13:23:23] ✅ Found corresponding APK: com.PuzzlePoint.IdleRPG.apk
[13:23:23] 📱 Using APK for decompilation: com.PuzzlePoint.IdleRPG.apk
[13:23:23] ⚙️ Do not decode sources: ✅ Enabled (faster, no smali)
[13:23:23] 🔧 Starting APK decompilation with APKTool...
[13:23:23] 📤 I: Using Apktool 2.11.0 on com.PuzzlePoint.IdleRPG.apk with 8 threads
[13:23:23] 📤 I: Copying raw classes.dex file...
[13:23:23] 📤 I: Copying raw classes2.dex file...
[13:23:23] 📤 I: Loading resource table...
[13:23:23] 📤 I: Decoding file-resources...
[13:23:23] 📤 I: Loading resource table from file: C:\Users\y\AppData\Local\apktool\framework\1.apk
[13:23:24] 📤 I: Decoding values */* XMLs...
[13:23:24] 📤 I: Decoding AndroidManifest.xml with resources...
[13:23:24] 📤 I: Regular manifest package...
[13:23:24] 📤 I: Copying original files...
[13:23:24] 📤 I: Copying assets...
[13:23:25] 📤 I: Copying lib...
[13:23:25] 📤 I: Copying kotlin...
[13:23:25] 📤 I: Copying unknown files...
[13:23:25] 🔚 Process exit code: 0
[13:23:25] ✅ APK decompilation completed successfully
[13:23:25] 📊 Decompilation Results:
[13:23:25] ========================
[13:23:25] ✅ AndroidManifest.xml - App configuration
[13:23:25] ✅ lib/ - Native libraries (1 architectures)
[13:23:25]    📱 arm64-v8a: 7 .so files
[13:23:25] ⚡ Sources skipped (--no-src flag used)
[13:23:25] 💡 Faster decompilation, no smali code generated
[13:23:25] 📁 Total: 1213 files extracted
[13:23:25] ========================
[13:23:25] 🔧 Applying post-decompilation fixes...
[13:23:25] 🔧 Post-Decompilation Fixes:
[13:23:25] ==========================
[13:23:25]    ℹ️ AndroidManifest.xml already clean, no fixes needed
[13:23:25]    ℹ️ apktool.yml already configured correctly
[13:23:25]    ℹ️ Processed 10 files, no dummy entries found
[13:23:25] 🎯 Applied 0 post-decompilation fixes
[13:23:25] 💡 These fixes prepare the APK for successful recompilation
[13:23:25] ==========================
[13:23:25] 🎯 APK decompiled successfully to: com.PuzzlePoint.IdleRPG
[13:23:25] 📋 Metadata extraction, decompilation and post-processing completed. Files ready for analysis and recompilation.
[13:23:25] ========================================
[13:23:25] ✅ APK decompilation completed successfully!


16.  (CheckBox)
Name: "Do not Decode Sources"
Properties: Checked = true (default)
Location: Next to Decompile button
Actions:  (state flag)
What It Does: Controls whether APKTool should skip source code decoding during decompilation to save time


17.  (Button)
Name: "Dump"
Location: Next row
Actions:
Click: Extracts game code and structures from APK
What It Does: Executes Python script to dump IL2CPP metadata and code from decompiled APK

Example Running: 
[13:36:01] 🚀 Starting IL2CPP Dump Process...
[13:36:01] ========================================
[13:36:01] 🔍 Detecting AmpedGems structure...
[13:36:01] 📁 Detected structure: New (tools folder)
[13:36:01] 🐍 Python path: O:\23-07-2025\AmpedGems\tools\Python\python.exe
[13:36:01] 🔧 Virtual environment: O:\23-07-2025\AmpedGems\tools\Py_env
[13:36:01] 📜 Script path: O:\23-07-2025\AmpedGems\tools\Py_scripts\2.py
[13:36:01] ✅ Validating paths...
[13:36:01] ⚙️ Setting up environment variables...
[13:36:01] 🔥 Executing IL2CPP Dump Script...
[13:36:01] 🔧 Executing: O:\23-07-2025\AmpedGems\tools\Py_env\Scripts\python.exe "O:\23-07-2025\AmpedGems\tools\Py_scripts\2.py"
[13:36:01] 📁 Working directory: O:\23-07-2025\AmpedGems\tools\Py_scripts
[13:36:02] 📤 [░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░] 0% - Starting decompilation workflow
[13:36:02] 📤 [█░░░░░░░░░░░░░░░░░░░░░░░░░░░░░] 5% - Using architecture preference: 64
[13:36:02] 📤 [███░░░░░░░░░░░░░░░░░░░░░░░░░░░] 10% - Processing architecture folders
[13:36:02] 📤 [██████░░░░░░░░░░░░░░░░░░░░░░░░] 20% - Finding necessary files
[13:36:02] 📤 [█████████░░░░░░░░░░░░░░░░░░░░░] 30% - Starting Il2CppDumper
[13:36:04] 📤 [████████████░░░░░░░░░░░░░░░░░░] 40% - Processing with Il2CppDumper
[13:36:26] 📤 [██████████████████░░░░░░░░░░░░] 60% - Il2CppDumper processing completed successfully
[13:36:26] 📤 [█████████████████████░░░░░░░░░] 70% - Preparing DnSpy (killing existing instances).
[13:36:26] 📤 [██████████████████████░░░░░░░░] 75% - Starting DnSpy
[13:36:29] 📤 [████████████████████████░░░░░░] 80% - Opening files in DnSpy
[13:36:37] 📤 [███████████████████████████░░░] 90% - DnSpy automation completed
[13:36:37] 📤 [██████████████████████████████] 100% - Workflow completed successfully
[13:36:37] 📤 
[13:36:37] 📤 Script completed in 34.88 seconds
[13:36:37] 🏁 Script completed with exit code: 0
[13:36:37] ========================================
[13:36:37] ✅ IL2CPP dump process completed successfully!


18.  (Button)
Name: "Find Possible Functions"
Location: Next to Dump button
Actions:
#What It Does: # work in progress: (Intended to find possible functions to hook based on dump data, but not yet implemented)
 
19.  (NumericUpDown)
Properties: Minimum = 1, Value = 5
Location: Next to Find Possible Functions button
Actions: User can change value
What It Does: Controls how many top functions to find/display when Find Possible Functions is implemented


20.  (CheckBox)
Name: "Bypass Old Pairip"
Properties: Checked = true (default)
Location: Next row
Actions:  (state flag)
What It Does: Controls whether to apply old Pairip bypass during injection/recompilation

21.  (CheckBox)
Name: "Bypass Signature"
Properties: Checked = false (default)
Actions:  (state flag)
# What It Does: Work in progress : Controls whether to apply signature verification bypass during injection/recompilation

22.  (CheckBox)
Name: "Auto Recompile"
Properties: Checked = true (default)
Location: Next row
Actions:  (state flag)
What It Does: Controls whether to automatically recompile the APK after injecting empty menu

23.  (Button)
Name: "Inject Empty Menu"
Actions:
Click: Builds empty menu template and injects it into decompiled game
What It Does: Injects empty menu framework into the game, applies bypasses based on checkboxes, and optionally recompiles. Has failsafe mechanism to prevent re-execution.

Example Running: 
[13:37:27] 🔒 Created failsafe file - Inject Empty Menu button will remain disabled
[13:37:27] 🚀 Starting Build Empty Menu Process...
[13:37:27] ========================================
[13:37:27] 🔍 Detecting AmpedGems structure...
[13:37:27] 📁 Detected structure: New (tools folder)
[13:37:27] 📱 MainActivity value from textbox: com.unity3d.player.UnityPlayerActivity
[13:37:27] 🔒 Bypass Pairip enabled: True
[13:37:27] 📋 Copying orgmain Main.cpp to template...
[13:37:27] ✅ Main.cpp copied from orgmain to template
[13:37:27] ☕ Updating template MainActivity.java GameActivity field...
[13:37:27] 🔍 Found GameActivity line at index 10: 'public String GameActivity = "com.unity3d.player.UnityPlayerActivity";'
[13:37:27] 🔄 Original line: public String GameActivity = "com.unity3d.player.UnityPlayerActivity";
[13:37:27] 🔄 New line: public String GameActivity = "com.unity3d.player.UnityPlayerActivity";
[13:37:27] ✅ GameActivity line updated successfully!
[13:37:27] ✅ Template MainActivity updated to: com.unity3d.player.UnityPlayerActivity
[13:37:27] 🧹 Clearing template build folder for fresh build...
[13:37:27] ✅ Template build folder cleared for fresh build
[13:37:27] 🏗️ Building menu (using build first menu logic)...
[13:37:27] 🏗️ Starting build first menu process...
[13:37:27] 🔧 Running gradle build with environment setup...
[13:37:27] 🚀 Starting gradle build process...
[13:37:49] ✅ Gradle build completed successfully!
[13:37:49] ✅ Menu build completed successfully
[13:37:49] 📁 Copying from build location to workspace...
[13:37:49] 📁 Copying build output to workspace...
[13:37:49] ✅ Fresh APK copied to workspace: app-debug.apk
[13:37:49] 📅 APK build time: 2025-09-30 13:37:48
[13:37:49] 📦 Package name from .cpp marker: com.PuzzlePoint.IdleRPG
[13:37:49] 📦 Package name: com.PuzzlePoint.IdleRPG
[13:37:49] ✅ Found built APK: O:\23-07-2025\AmpedGems\workspace\app-debug.apk
[13:37:49] 📱 Using built APK: app-debug.apk
[13:37:49] 📦 Extracting APK to temp folder...
[13:37:49] ✅ APK extracted to temp folder: O:\23-07-2025\AmpedGems\workspace\temp_extraction
[13:37:49] 🔍 Validating ARM64 architecture requirements...
[13:37:49] 🔍 Architecture scan: ARM64=True, ARM32=False
[13:37:49] ✅ ARM64 architecture confirmed - Inject Empty Menu can proceed
[13:37:49] 🔄 Processing extracted files (ARM64 only)...
[13:37:49] 📊 Found 2 existing DEX files in game folder (highest: 2)
[13:37:49] 📦 Found 1 DEX files in app-debug.apk
[13:37:49] ✅ Copied classes.dex → classes3.dex (53620 bytes)
[13:37:49] ✅ Successfully added 1 DEX files: classes3.dex
[13:37:49] ✅ Copied ARM64 libraries: libAmpedGems.so
[13:37:49] ✅ Processed extracted APK files
[13:37:49] 📝 Applying manifest modifications...
[13:37:49] ✅ Manifest modifications applied
[13:37:49] ✅ Build empty menu workflow completed successfully!
[13:37:49] 🧹 Cleaned up temporary extraction folder
[13:37:49] ========================================
[13:37:49] ✅ Build empty menu process completed successfully!

24.  (Button)
Name: "Recompile Normally"
Actions:
Click: Recompiles decompiled APK back into installable APK file
What It Does: Recompiles APK using APKTool with default settings, zipaligns, and signs the APK for installation

Example Running:
[13:37:49] 🚀 Starting Auto Recompilation...
[13:37:49] 🔍 Detecting AmpedGems structure...
[13:37:49] 📁 Detected structure: New (tools folder)
[13:37:49] 🔍 Looking for .cpp marker file in workspace...
[13:37:49] 📄 Found marker file: com.PuzzlePoint.IdleRPG.cpp
[13:37:49] 📦 Package name: com.PuzzlePoint.IdleRPG
[13:37:49] 📂 Target decompiled folder: com.PuzzlePoint.IdleRPG
[13:37:49] ✅ All required tools found
[13:37:49] 🔨 Starting APK compilation with default settings...
[13:37:49] ================================================
[13:37:49] 🧹 Cleaning up problematic files from previous runs...
[13:37:49]    ✅ No problematic files found
[13:37:49] 📋 Extracting APK metadata for naming...
[13:37:49] 📄 Found version file: 42.0.0.version
[13:37:49] 📊 Extracted version: 42.0.0
[13:37:49] 📂 Input folder: com.PuzzlePoint.IdleRPG
[13:37:49] 📱 App: Go Hero Go v42.0.0
[13:37:49] 📦 Final APK: Go_Hero_Go_42.0.0.apk
[13:37:49] 🔍 Decompiled with: APKTool
[13:37:49] 🔨 Building APK...
[13:37:57] ✅ APK compilation completed: com.PuzzlePoint.IdleRPG compiled.apk
[13:37:57] ⚡ Zipaligning APK...
[13:37:57] ✅ Zipalign completed
[13:37:57] 🔐 Signing APK...
[13:37:58] ✅ APK signing completed
[13:37:58] 🔍 Debug - toolsPath: O:\23-07-2025\AmpedGems\tools\apktool
[13:37:58] 🔍 Debug - ampedGemsBase: O:\23-07-2025\AmpedGems
[13:37:58] 🔍 Debug - updatedDir: O:\23-07-2025\AmpedGems\updated
[13:37:58] 📋 Copying final APK to updated directory: O:\23-07-2025\AmpedGems\updated\Go_Hero_Go_42.0.0.apk
[13:37:58] ✅ Final APK copied to: updated/Go_Hero_Go_42.0.0.apk
[13:37:58] 🧹 Deleted .idsig file
[13:37:58] 🧹 Cleaned up compiled APK
[13:37:58] 🧹 Cleaned up zipaligned APK
[13:37:58] ================================================
[13:37:58] 🎉 APK compilation successful! Output: Go_Hero_Go_42.0.0.apk
[13:37:58] ========================================
[13:37:58] ✅ Auto recompilation completed successfully!
[13:37:58] 🎉 Complete workflow finished! Empty menu injected and APK recompiled.
[13:37:58] 🔒 Inject Empty Menu button permanently disabled to prevent re-execution


25.  (RichTextBox)
Properties: BackColor = Light Gray, Dock = Bottom, Size = 197px height
Location: Docked at bottom of tab
Actions:  (display only)
What It Does: Displays timestamped log messages for all Phase 1 operations, providing real-time feedback to the user
