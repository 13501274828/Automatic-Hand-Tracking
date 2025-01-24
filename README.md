
# Automatic Hand Tracking with SAM

This project implements automatic hand tracking in videos using SAM2. It detects and masks hands in each frame of a video and outputs the processed video.

## Features
- **Hand Detection**: Detects hand locations in video frames.
- **Hand Masking**: Generates segmentation masks for detected hands using SAM.
- **Video Processing**: Outputs a processed video with hands masked.

## Prerequisites
- Python 3.8 or higher
- NVIDIA GPU with CUDA support (recommended for faster processing)

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-repo/automatic-hand-tracking.git
   cd automatic-hand-tracking
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Download the SAM checkpoint:

   ```bash
   wget -O sam_vit_b.pth https://dl.fbaipublicfiles.com/segment_anything/sam_vit_b_01ec64.pth
   ```

## Usage

1. Prepare your input video and place it in the project directory.

2. Run the script to process the video:

   ```bash
   python hand_tracking.py --input_path <input_video_path> --output_path <output_video_path>
   ```

   Replace `<input_video_path>` with the path to your input video and `<output_video_path>` with the desired output path.

3. The processed video with masked hands will be saved at the specified output location.

## Dependencies
See `requirements.txt` for a list of dependencies.

## Acknowledgements
This project utilizes [Segment Anything Model (SAM)](https://github.com/facebookresearch/segment-anything) by Facebook Research.
