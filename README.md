# JULIUS - Contnious Speech Recongition System
---------------------------------------------

# ABOUT 
"Julius" is a high-performance, small-footprint large vocabulary continuous 
speech recognition (LVCSR) decoder software for speech-related researchers 
and developers.The algorithm is based on 2-pass tree-trellis search, which 
fully incorporates major decoding techniques such as tree-organized lexicon, 
1-best / word-pair context approximation, rank/score pruning, N-gram 
factoring, cross-word context dependency handling, enveloped beam search, 
Gaussian pruning, Gaussian selection, etc. 
The main platform is Linux and other Unix-based system, as well as Windows, 
Mac, Androids and other platforms.


# HOW TO RUN 

## 1. Install julius(linux)
    sudo apt-get install build-essential zlib1g-dev libsdl2-dev libasound2-dev
    sudo apt-get install julius
    or
    sudo apt-get install build-essential zlib1g-dev libsdl2-dev libasound2-dev
    git clone https://github.com/julius-speech/julius.git
    cd julius
    ./configure --enable-words-int
    make -j4
    or 
    download julius-4.3.1.tar.gz and extract it
    run run_install.sh 
## 2. Download the Trained model 
    git clone https://github.com/ImAshishRastogi/julius.git
    
    Note: To Train your own model Go to Link : https://github.com/ImAshishRastogi/julScript
## 3. FILELIST
    contain the path of each wav file.

## 4. Sample.jconf
    Path - julius/model/sample.jconf
    
## 5. Run Julius with trained model on CLI
    julius -input rawfile -filelist (FILELIST) -C (Path of .jconf file from trained model) -output

