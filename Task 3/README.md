# 🎼 Task 3: Music Generation with AI  

## 📋 Project Overview  
This project implements an **AI-powered Music Generation system** using deep learning.  
The model is trained on MIDI files and learns to generate new, original music sequences.  
The system can output melodies in **MIDI format** (for editing/arranging) and can also be converted into **playable audio (WAV)** using FluidSynth with a SoundFont.  

---

## 🚀 Features  
- 🎶 Train a deep learning model on MIDI music files  
- 🎹 Generate new original music sequences  
- 📂 Save generated music as `.mid` files  
- 🔊 Convert MIDI to WAV for playback  
- 🌐 Interactive **Gradio Interface** for real-time music generation  

---

## 🛠️ Tech Stack  
- **Python**  
- **TensorFlow / Keras** – Model training  
- **Music21** – MIDI parsing and preprocessing  
- **PrettyMIDI** – MIDI manipulation  
- **PyFluidSynth + SoundFonts** – MIDI to WAV conversion  
- **Gradio** – Web-based interface  

---

## 📂 Dataset  
The model is trained on a collection of **MIDI files**.  
Each file is parsed into note sequences, which are then used to train the neural network.  

---

## ⚙️ Installation & Setup  

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/music-generation-ai.git
   cd music-generation-ai

Install dependencies:

pip install -r requirements.txt


(Optional for audio output) Install FluidSynth:

# Ubuntu/Colab
sudo apt-get install -y fluidsynth

# macOS (via Homebrew)
brew install fluidsynth


Download a SoundFont (e.g., FluidR3 GM) for MIDI-to-WAV conversion:

wget https://github.com/urish/cyberbot/raw/master/resources/soundfonts/FluidR3_GM.sf2 -O FluidR3_GM.sf2

▶️ Usage
🔑 Train & Save Model

After training, save the model and note mappings:

model.save("music_model.keras")

with open("note_mappings.pkl", "wb") as f:
    pickle.dump(int_to_note, f)

🎶 Generate Music
from tensorflow.keras.models import load_model
import pickle

# Load model
model = load_model("music_model.keras")

# Load mappings
with open("note_mappings.pkl", "rb") as f:
    int_to_note = pickle.load(f)

# Generate new MIDI
generated_music = generate_music(model, int_to_note, length=200)

🔊 Convert MIDI to WAV
import pretty_midi, soundfile as sf

midi_data = pretty_midi.PrettyMIDI("generated_music.mid")
audio_data = midi_data.fluidsynth(sf2_path="FluidR3_GM.sf2")
sf.write("generated_music.wav", audio_data, 44100)

🌐 Run Gradio Interface
import gradio as gr

def generate_and_play():
    # Music generation code
    return "generated_music.wav"

gr.Interface(fn=generate_and_play, inputs=None, outputs="audio").launch()

📊 Results

Successfully trained a model to learn from MIDI sequences

Generated unique music compositions

Enabled real-time playback through Gradio

🎥 Demo

📺 Include a link here if you record a demo video of generated music