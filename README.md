# dotFiles
#
#Compiling vim from source for MAC with Ruby, Python, and Perl support

git clone https://github.com/vim/vim.git
cd vim/src/
./configure --with-features=huge \
            --prefix=/opt/vim \
            --enable-multibyte \
            --enable-rubyinterp=yes \
            --enable-pythoninterp=yes \
            --enable-python3interp=yes \
            --enable-perlinterp=yes
sudo make && sudo make install && sudo make clean
