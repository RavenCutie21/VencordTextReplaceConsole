This is good enough for me so uhh cope, seethe, mald, copy everything, paste it on like gdocs and expand, should get through like 70% of all help related stuff from this already. have a nice day stinkers

this is also for the clueless people tbh who just get dragged into it without knowing what the fuck is going on, or also if you are just very lazy

# Helping-in-AI-Hub (voice changer section)

## Most things here are just common things compiled from my guide and Antasma's pages.

### Feel free to copy this elsewhere like gdocs and add the Training/Cover stuff or DM me what to add [@ravencutie21](https://discord.com/users/824922747423031359) 



### If at any point you don't know something or are busy
tell them to look in #info & #how-to-use, pins, or link them the guides yourself if you think they can not find pins


### Two things to ask immediately

Ask : What is your GPU?
* Depending on answer Please change how you are going to recommend stuff
* link this https://github.com/YunaOneeChan/Voice-Changer-Settings#what-version-to-download as it has a direct download to the correct version at all times, or what is arguably idiot proof, copy the correct link from that section and send it to them
* If the gpu does not have at least 8gb of V-Ram they are better off using Colab
  
Ask: What are your voice changer settings (screenshot) 
* NVIDIA : Set your F0. to RMVPE if it has issues use CREPE_TINY, set your chunk to 112, if it isn't a clear voice or is stuttering go to 192, set your extra to 8192 or a maximum of 32768, this increases CPU the higher it is.
* AMD or INTEL ARC : Set your F0. to RMVPE_ONNX if it has issues use CREPE_TINY, set your chunk to 112, if it isn't a clear voice or is stuttering go to 192, set your extra to 8192 or a maximum of 32768, this increases CPU the higher it is, set your GPU to GPU0 as 99% of the time it will be your graphics card. You can verify in Task manager under the performance tab. Also remember to EXPORT model to ONNX and reupload that new file
* Colab : Set your F0. to RMVPE_ONNX, set your chunk to 112, set your extra to 8192.
* As far as I can tell, there is zero reason to go higher than 32768; unless you have a weird anomaly like (Haien) where his does not work unless his extra is higher.

### They will tell you these things (wip still adding more) 

If told start_http.bat instantly closes : 
* Have them look at pins, there is a video there
* If they are one Win 11, instead of clicking the top bar, tell them to right click in the empty space of the folder and press "Open in terminal", and continue watching the video.

If told only default models are clear, and or uploaded models are not,
* They are likely to be on an AMD or ARC card, tell them to EXPORT TO ONNX, and UPLOAD the new file that was created

If there is Any Connection Error, or Wait for Server :
* stored_setting.json is likely the culprit deleting this will usually fix it
* or their firewall / av is blocking it

If they ask how to use the Colab version :
* refer to antasma's pin or just send link below
* https://docs.google.com/document/d/e/2PACX-1vTIceEcBfS6Zqolv_QEysrFfI_EJikPxozWptP_EjkpLVl-l-gdo-ijBonQMTviAHEYm5emmd9k9TdC/pub

If asked how do i use it elsewhere
* explain they need a virtual cable
* the output in the voice changer will be said virtual cable (Line 1 or VB-Audio Virtual Cable INPUT)
* the input on whatever they want to use it on will be said virtual cable (Line 1 or VB-Audio Virtual Cable OUTPUT)

If told voice changer isn't working ask
* do you have a virtual cable, if yes link them https://github.com/YunaOneeChan/Voice-Changer-Settings#virtual-cables
* is the passthru button red, if yes tell them to press it so it is green
* are you in server mode and is the CMD window saying false to any device, if yes your sample rates do not match for all of your devices in windows sound settings and what you picked in the voice changer
* its sending both my desktop audio and mic, they most likely need to install something else like Steelseries sonar, it is a bug when both devices are the same name as far as i can tell, sonar will split it so it shouldnt happen.

If told voice changer is speaking on it's own
* either link https://github.com/YunaOneeChan/Voice-Changer-Settings#noise-suppression
* or tell them to enable ONLY sup2, and raise s.threshhold

If a screenshot shows PIPELINE IS NOT INITIALIZED
* refer to Antasma's Pin for error fixes
* https://docs.google.com/document/d/e/2PACX-1vQIwJ3MVidhgEaXwWFl0xpVonVOVfneaNVADd7-NMWFgPIsfWWhG8NNqzQMsXDIOGlBIfxscoIm2_6I/pub
* or just tell them what to do : Try re-extracting the folder on the root of your main drive (C:\MMVCServerSIO) or directly on your desktop. as its most likely what it is.

If asked about crackling voice, ask : Is it only in discord or is it everywhere
* Everywhere fix : https://github.com/YunaOneeChan/Voice-Changer-Settings#audiodgexe-optimizations
* Discord fix : https://github.com/YunaOneeChan/Voice-Changer-Settings#discord-settings


# HEAVY WIP RVC section
Any colab with RVC in it's name dies, it is fully detected and actively getting banned just recommend people installing locally or unfortunately using something like kits.
move more people over to local install if you can and colab's will last significantly longer

also it is just against tos so uhh pay :3

Kaggle is what everyone is going to now since colab is banned


HOW LOCAL INSTALL
* https://github.com/IAHispano/Applio-RVC-Fork (seems to be the most up to date, never used, what everyone uses on colab)
* https://huggingface.co/MangioRVC/Mangio-RVC-Huggingface/tree/main + https://github.com/MrFelt/F-RVC (better defaults over mangio and just looks better)
* https://huggingface.co/lj1995/VoiceConversionWebUI/tree/main Official local (what i use also has better voice changer performance for amd & intel people)


Epoch to go for?
* there is no correct answer, just put a big number you dont think youd reach
* just watch tensorboard and when you see "overtraining" you stop

How make model or dataset for training
* get audio, uvr it, any _ft model usually is best unless you are uvring multiple times, throw in audacity, process however you want, then
* truncate silence @ -40db or whatever still has your voice, -0.05 length or greater, to -0.05, that is now your dataset. truncate silence is mandatory on large datasets
* open rvc either colab (applio) or local install, and just do it


HOW MAKE COVER
* Lazy way instead of Applio, Link SociallyIneptWeebs AI Cover Gen, it is the easiest way to do this.
* full link : https://github.com/SociallyIneptWeeb/AICoverGen
* colab specific link : https://colab.research.google.com/github/SociallyIneptWeeb/AICoverGen/blob/main/AICoverGen_colab.ipynb

