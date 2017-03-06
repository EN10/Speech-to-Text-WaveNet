Convert Audio:
http://superuser.com/questions/23930/how-to-decode-aac-m4a-audio-files-into-wav

ImportError: No module named
sudo -H pip install

If Dependencies are installed as described then it works!
Seems to brake with newer dependencies installed.
Used: pip freeze to see which version installed.
If a newer version is installed then uninstall: sudo pip uninstall sugartensor
Then install correct version: sudo pip install sugartensor==0.0.1.9
Tensorflow version: sudo pip show tensorflow
To install correct version of tensorflow:
sudo pip install https://storage.googleapis.com/tensorflow/linux/cpu/tensorflow-0.11.0-cp27-none-linux_x86_64.whl