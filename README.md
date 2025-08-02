# HIK Vision Traffic Sign AI Toolkit

🚗 **Extract, Test, and Rebuild HIK Vision dashcam firmware with traffic sign AI**

## Compatible Camera Model

**AE-DC5013-F6PRO - 1600P Dashcam with GPS**

- Up to 1600P high resolution, gold wide angle up to 130°
- F1.6 super large aperture offer a perfect night image  
- Support built-in MIC and speaker for audio in and out
- Built-in WIFI module and WIFI AP function supported
- Built-in G-Sensor module, support video recording linkage at car crash or strong vibration (Linkage video record can be configured be no-overwritten)
- Support GPS module with speed display and route tracking playback
- Micro SD card for video recording, up to 256GB (Overwriting supported)
- Phone App: live view, record playback and parameter configuration
- Voice recognition supported: Snapshot, Recording on, Recording off
- **ADAS supported**: "Traffic light turn green", "Speed limit recognition", "Front car start remind"
- Easy installation and user friendly, plug and play (Automatically recording after power on)
- Low power consumption and high performance

## Quick Start

1. Place your `digicap.dav` firmware file in this directory
2. Run: `python3 HIK_Traffic_AI_Toolkit.py`
3. Choose option 1 (Complete Pipeline)
4. Follow the prompts

## What It Does

- **Extracts** 483MB traffic sign AI model from firmware
- **Tests** the AI using your webcam (real-time detection)
- **Rebuilds** firmware with your modifications
- **Preserves** original firmware safely

## Project Structure

```
HIK_Traffic_AI_Clean/
├── HIK_Traffic_AI_Toolkit.py    # Main program (run this)
├── webcam_tester.py             # Testing module  
├── digicap.dav                  # Original firmware
├── ai_model/traffic_signs.bin   # Extracted 483MB AI
├── firmware_backup/             # Safe backup
├── firmware_output/             # Modified firmware
└── test_results/                # Detection samples
```

## Requirements

- Python 3.x
- OpenCV: `sudo apt install python3-opencv python3-numpy python3-pil`
- Webcam for testing

## Usage

```bash
python3 HIK_Traffic_AI_Toolkit.py
```

**Menu Options:**
1. Complete Pipeline (recommended)
2. Extract AI only
3. Test with webcam only  
4. Rebuild firmware only
5. Show status

## Safety

✅ Original firmware never modified  
✅ Automatic backups created  
✅ All operations reversible  
✅ Clean file organization  

Perfect for dashcam customization and AI research!
