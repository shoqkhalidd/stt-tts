# stt-tts

## Description

this project is a tool to convert speech to text then test to speech using IBM watson

the speech to text was cloned [from](https://github.com/nicknochnack/RealTimeSpeechToText/tree/main/watson-streaming-stt) please check it out to understand how it works

for the text to speech part 
in the tts() methods make sure to change the apikeys and the url for it to work 

## Requirements 

- pyaudio
- websocket-client
- ibm_watson
- playsound

or by using 
```
pip3 install -r requirements.txt 
```
## Running 

use 
```
python3 transcribe.py -t  
```
after -t please choose the time you want to record

## Output

the result of STT can be seen [here](res.txt) 
and the result of the TTS can be heard [here](speech.mp3)
