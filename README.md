# stt-tts-chatbot

## Description

this project is an audio chatbot it works by using IBM Watsons' speech to text,watson's assistant as well as text to speech services.

## how it works
it will take the text created by STT into the chatbot to get the response then the TTS will play the response from said chatbot.

please make sure to change the apikeys and the url for it to work.

#### note:
the speech to text was cloned [from here](https://github.com/nicknochnack/RealTimeSpeechToText/tree/main/watson-streaming-stt) please check it out to understand how it works the only diffrence is that here it's saved into a [text file](stt.text) as a proof for it to be working.

the chatbot is using the same assistant [here](https://github.com/shoqkhalidd/chatbot).

for the text to speech part 
in the tts() methods
first it'll read the sentence that was made by the chatbot aka the res.ttx it'll synthesize said text into a [mp3 file](speech.mp3) as a response.

#### note:
the voice of the narrator can be changed [here](https://cloud.ibm.com/docs/text-to-speech?topic=text-to-speech-voices).

## Requirements 

- pyaudio
- websocket-client
- ibm_watson
- playsound

or by using 
```
pip3 install -r requirements.txt 
```
## To run 

use 
```
python3 transcribe.py -t  
```
after -t please choose the time you want to record.

## Output

the result of STT can be seen [here](stt.txt), fot the chatbot it can be seen [here](res.txt) 
and the result of the TTS can be heard [here](speech.mp3).
