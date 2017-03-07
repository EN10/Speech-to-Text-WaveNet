#Speech-to-Text-WaveNet#

Based on: https://github.com/buriburisuri/speech-to-text-wavenet  
With file dependancies and pre-trained model in assets folder for recognize.py    

Dependencies
-
The original dependancies are not 100% correct, as described here:  
https://github.com/buriburisuri/speech-to-text-wavenet#dependencies     
It seems to break with newer versions of tensorflow or sugartensor.   

My Updated Dependancies File:  https://github.com/EN10/STT/blob/master/requirements.txt    

Working Dependancies
-
Works with:     
pandas 0.19.2 (latest)  
librosa to 0.5.0 (latest)   
tqdm to 4.11.2 (latest)     
tensorflow 1.0.0, 0.12.1 & 0.12.0 doesn't work, only tensorflow 0.11.0.  
sugartensor version > 0.0.1.9 doesn't work, only 0.0.1.9 does.   

Changing Dependancies
-
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


Other Issues
-

ImportError: No module named  

    sudo -H pip install
    
Convert Audio:  
http://superuser.com/questions/23930/how-to-decode-aac-m4a-audio-files-into-wav