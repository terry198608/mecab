# mecab Documentation
[Offical Documentation](https://taku910.github.io/mecab/)

# Install MeCab
**Linux**  
  
Linux users can more than likely find MeCab in their distro repositories. Simply install 'mecab' and the package 'mecab-ipadic-utf8'. Ubuntu users can do this with the following command.  

`sudo apt-get install mecab mecab-ipadic-utf8`  
    
If that doesn't work, you can download the source and build it yourself. Note that this will require the package 'build-essential'.  
First pull in MeCab.  
  `wget https://mecab.googlecode.com/files/mecab-0.996.tar.gz  
  tar zxfv mecab-0.996.tar.gz  
  cd mecab-0.996  
  ./configure --with-charset=utf8 --enable-utf8-only`  
    
Then get the dictionary file.  
  `wget https://mecab.googlecode.com/files/mecab-ipadic-2.7.0-20070801.tar.gz  
  tar zxfv mecab-ipadic-2.7.0-20070801.tar.gz  
  cd mecab-ipadic-2.7.0-20070801  
  ./configure --with-charset=utf8`  
  
**Mac OS X**  
Both MeCab and the required dictionary (mecab-ipadic-utf8) are in MacPorts. If that doesn't work, try downloading the source and building it yourself. You can get the source and the dictionary from the following urls:  
  
https://mecab.googlecode.com/files/mecab-0.996.tar.gz  
https://mecab.googlecode.com/files/mecab-ipadic-2.7.0-20070801.tar.gz  
  
**Windows**  
Download the installer from this url: https://mecab.googlecode.com/files/mecab-0.996.exe  
  
Once you get mecab to start, type some Japanese and make sure you get an appropriate response.  

  `~$ mecab  
  やった  
  やっ    動詞,自立,*,*,五段・ラ行,連用タ接続,やる,ヤッ,ヤッ  
  た      助動詞,*,*,*,特殊・タ,基本形,た,タ,タ  
  ！      記号,一般,*,*,*,*,！,！,！  
  EOS`  
