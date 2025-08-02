# HIK Vision Traffic Sign AI Toolkit

🚗 **Extract, Test, and Rebuild HIK Vision dashcam firmware with traffic sign AI**

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
