FROM debian

RUN apt-get update && apt-get install -y gcc autotools-dev automake flex bison libglib2.0-dev libvirt-dev libjson-c-dev libyajl-dev git libtool make
RUN git clone https://github.com/libvmi/libvmi && \
    cd libvmi && \
    ./autogen.sh && \
    ./configure && \
    make && \
    make install && \
    ldconfig



