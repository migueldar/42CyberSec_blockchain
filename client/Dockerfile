FROM debian

RUN apt-get update
RUN apt-get install -y build-essential libreadline-dev unzip wget git
#lua
RUN wget http://www.lua.org/ftp/lua-5.4.4.tar.gz
RUN tar -zxf lua-5.4.4.tar.gz
RUN cd lua-5.4.4; make linux test; make install
#luarocks
RUN wget https://luarocks.org/releases/luarocks-3.9.1.tar.gz
RUN tar -zxf luarocks-3.9.1.tar.gz
RUN cd luarocks-3.9.1; ./configure; make install
#RUN luarocks install lua-requests

CMD tail -f /dev/null