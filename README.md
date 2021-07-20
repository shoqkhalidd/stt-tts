# stt-tts

## Description

this project is a tool to convert speech to text then test to speech using IBM watson

the speech to text was cloned [from here](https://github.com/nicknochnack/RealTimeSpeechToText/tree/main/watson-streaming-stt) please check it out to understand how it works the only diffrence is that here it's saved into a [text file](res.text)

for the text to speech part 
in the tts() methods make sure to change the apikeys and the url for it to work 
first it'll read the sentence that was made by the stt aka the res.ttx it'll synthesize said text to a speech 
note the voice of the narrator can be changed [here](https://cloud.ibm.com/docs/text-to-speech?topic=text-to-speech-voices)

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
