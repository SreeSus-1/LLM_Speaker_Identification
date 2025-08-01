# LLM_Speaker_Identification
Identifying the speaker through audio using Gen AI


🎙️ Notebook: LLM_Speaker_Identification.ipynb
This notebook builds a speaker analysis pipeline from a YouTube video using the following:

📌 Key Features
Downloads and extracts audio using pytube and pydub

Splits long audio into smaller chunks for processing

Performs speaker diarization with pyannote.audio from Hugging Face

Identifies gender (using a placeholder function)

Summarizes total, male, and female speakers

🔧 Libraries Used
pytube, pydub, pyannote.audio

torch, torchaudio, numpy

🧠 Defined Functions
download_and_convert_video(video_url): Downloads audio from a YouTube link

split_audio(wav_path): Splits WAV into 20-second chunks

diarize_speakers(audio_path): Uses pretrained pipeline to label speaker segments

identify_gender(segment): Dummy function (can be improved)

process_diarization(diarization, audio_path): Applies gender ID to each speaker

summarize_speakers(speaker_genders): Prints count by gender and speaker
