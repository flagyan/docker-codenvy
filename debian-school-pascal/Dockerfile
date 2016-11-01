FROM codenvy/debian_jre

RUN sudo apt-get update && \
    sudo apt-get -y install g++ gcc make gdb gdbserver fp-compiler vim && \
    sudo apt-get clean && \
    sudo apt-get -y autoremove && \
    sudo rm -rf /var/lib/apt/lists/*

RUN echo "alias l=\"ls -lhatp --color\"" |sudo tee -a /home/user/.bashrc
RUN echo "alias ll=\"ls -lhatp --color\"" |sudo tee -a /home/user/.bashrc
RUN echo "alias l=\"ls -lhatp --color\"" |sudo tee -a /home/user/.bashrc

RUN echo "alias gi=\"git init\"" |sudo tee -a /home/user/.bashrc
RUN echo "alias gs=\"git status\"" |sudo tee -a /home/user/.bashrc
RUN echo "alias gc=\"tee .git-commit <<EOF; git commit -F .git-commit; rm .git-commit\"" |sudo tee -a /home/user/.bashrc
RUN echo "alias gca=\"git commit --amend\"" |sudo tee -a /home/user/.bashrc
RUN echo "alias gcl=\"git clone\"" |sudo tee -a /home/user/.bashrc
RUN echo "alias ga=\"git add\"" |sudo tee -a /home/user/.bashrc
RUN echo "alias gaa=\"git add .\"" |sudo tee -a /home/user/.bashrc
RUN echo "alias gp=\"git push -u\"" |sudo tee -a /home/user/.bashrc

RUN git config --global user.email "xervondev@gmail.com"
RUN git config --global user.name "Mika Dede"

WORKDIR /projects

CMD tail -f /dev/null