<div align="center">

<h1>easyGUI</h1>
A fork of Retrieval based Voice Conversion WebUI <br><br>



# INSTALLATION termux



pkg update -y && pkg install wget curl proot tar -y && wget https://raw.githubusercontent.com/AndronixApp/AndronixOrigin/master/Installer/Ubuntu22/ubuntu22.sh -O ubuntu22.sh && chmod +x ubuntu22.sh && bash ubuntu22.sh


apt update -y && apt dist-upgrade -y && apt install wget curl git python3.10 python3-pip gcc python3-dev python3.10-venv ffmpeg libx11-dev -y; git config --global http.postBuffer 2097152000 && git config --global https.postBuffer 2097152000; echo "127.0.0.1 localhost" >> /etc/hosts; pip install virtualenv && virtualenv ez && source ez/bin/activate && python -m pip install pip==24.0; git clone https://github.com/RejektsAI/easyGUI && sed -i '/praat-parselmouth/d' easyGUI/requirements.txt && wget -O praat_parselmouth-0.4.4-cp310-cp310-linux_aarch64.whl "https://huggingface.co/Nick088/termux-built-arm64-files/resolve/main/pre-built-wheels/praat_parselmouth-0.4.4-cp310-cp310-linux_aarch64.whl?download=true" && pip3.10 install praat_parselmouth-0.4.4-cp310-cp310-linux_aarch64.whl && pip install -r easyGUI/requirements-android.txt


 

# RUN THE EASYGUI (from zero)


./start-ubuntu22.sh This is how you start UBUNTU (think of it like starting your computer)

source ez/bin/activate This is how you enter the environment

cd easyGUI This is how you enter the easyGUI folder

python mobile.py This is how you start the easyGUI


Or just copy and paste this whenever you just started Termux:


./start-ubuntu22.sh; source ez/bin/activate; cd easyGUI && python mobile.py





## Credits
+ [RVC](https://github.com/RVC-Project/Retrieval-based-Voice-Conversion-WebUI)
+ [ContentVec](https://github.com/auspicious3000/contentvec/)
+ [VITS](https://github.com/jaywalnut310/vits)
+ [HIFIGAN](https://github.com/jik876/hifi-gan)
+ [Gradio](https://github.com/gradio-app/gradio)
+ [FFmpeg](https://github.com/FFmpeg/FFmpeg)
+ [Vocal pitch extraction:RMVPE](https://github.com/Dream-High/RMVPE)
+ The pretrained model is trained and tested by [yxlllc](https://github.com/yxlllc/RMVPE) and [RVC-Boss](https://github.com/RVC-Boss).
