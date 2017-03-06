#Speech-to-Text-WaveNet#

Based on: https://github.com/buriburisuri/speech-to-text-wavenet  

Install
-

If Dependencies are installed as described then it works!   
Seems to break with newer dependencies installed.   
For Dependancies see:  

    requirements.txt

To see which version installed use:    

    pip freeze
    pip show tensorflow

If a newer version is installed then uninstall: 

    sudo pip uninstall sugartensor

Then install correct version: 

    sudo pip install sugartensor==0.0.1.9

To install correct version of tensorflow: 

    sudo pip install https://storage.googleapis.com/tensorflow/linux/cpu/tensorflow-0.11.0-cp27-none-linux_x86_64.whl

Run
-

Use recognise using test file:  

    python recognize.py --file test.wav

Working Dependancies
-
Works with:     
pandas 0.19.2 (latest)  
librosa to 0.5.0 (latest)   
tqdm to 4.11.2 (latest)     
tensorflow 1.0.0, 0.12.1 & 0.12.0 doesn't work, only tensorflow 0.11.0.  
sugartensor version > 0.0.1.9 doesn't work, only 0.0.1.9 does.   

Other Issues
-

ImportError: No module named  

    sudo -H pip install
    
Convert Audio:  
http://superuser.com/questions/23930/how-to-decode-aac-m4a-audio-files-into-wav