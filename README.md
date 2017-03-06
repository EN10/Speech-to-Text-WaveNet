#Speech-to-Text-WaveNet#

Based on: https://github.com/buriburisuri/speech-to-text-wavenet  

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

Use recognise using test file:  

    python recognize.py --file test.wav

ImportError: No module named  

    sudo -H pip install
    
Convert Audio:  
http://superuser.com/questions/23930/how-to-decode-aac-m4a-audio-files-into-wav