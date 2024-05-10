FROM frankfang128/oh-my-docker:mangosteen

RUN rm -rf ~/.oh-my-zsh/ && \
    curl -L http://install.ohmyz.sh > install.sh && \
    sh install.sh && \
    git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting && \
    git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions

COPY .zshrc /root/.zshrc




