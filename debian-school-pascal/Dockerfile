FROM codenvy/debian_jre

RUN sudo apt-get update && \
    sudo apt-get install g++ gcc make gdb gdbserver fp-compiler vim -y && \
    sudo apt-get clean && \
    sudo apt-get -y autoremove && \
    sudo rm -rf /var/lib/apt/lists/*

WORKDIR /projects

CMD tail -f /dev/null