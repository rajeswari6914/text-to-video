# Text-to-Video Generation Project

## Project Overview
This project generates a short video from a text prompt using a pre-trained model from Hugging Face's `TextToVideoSDPipeline`. The video frames are generated based on the given text, and then combined into a video file. This project was completed in Google Colab without using Streamlit, and the output video is saved directly to the specified path.

## Model
The model used for this project is `damo-vilab/text-to-video-ms-1.7b`, a pre-trained text-to-video generation pipeline available on Hugging Face. The model generates frames based on text input and then assembles them into a video.

## Steps
1. Installed necessary libraries directly in Colab:
   - `torch`
   - `diffusers`
   - `opencv-python`
   - `transformers`
   
2. Defined the pipeline and generation functions to convert a text prompt into video frames.
   
3. Generated frames based on the text prompt using the `generate()` function.

4. Converted the frames into a video file using the `convert_to_video()` function.

5. Saved the output video in `.mp4` format.

## Usage

This project generates videos from text prompts using the `Text-to-Video` pipeline from Hugging Face. It is designed to run efficiently on a machine with GPU support, such as Google Colab or any CUDA-enabled machine. Below are the steps to execute the code and generate a video from a text input.

## Steps to Run

1. Clone the repository and navigate to the project directory:
   
```bash
git clone <repository-link>
```
```bash
cd <repository-folder>
```
2. Open the text2video.ipynb notebook in Google Colab or Jupyter.
   
3. Install the necessary dependencies directly in the notebook:
   
```bash
!pip install torch diffusers opencv-python transformers
```
4. Authenticate with Hugging Face using your token (if required):
   
```bash
from huggingface_hub import login
login('your-huggingface-token')
```

5. Run the cells in the notebook to generate the video based on a text prompt.
   
7. The generated video will be saved as output_video.mp4 in the project directory.


## Example Input and Output

### Input
The following parameters were used for generating the video:

```python
prompt = "A cat playing with a ball"
num_frames = 16
num_steps = 50
seed = 42
height = 512
width = 512
```
### Output
The input prompt generated a video, saved as output_video.mp4. You can download or view the generated video here:



https://github.com/user-attachments/assets/6e3ca2c0-5a07-4106-ab5a-9d973951ad4c


[Download the generated video](https://github.com/rajeswari6914/text-to-video/blob/main/output_video%20(13).mp4)







