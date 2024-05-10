FROM custom_image

# RUN 1 | pacman -Syu
# RUN yes | pacman -S wget

# RUN useradd builduser


RUN rm -rf ~/.oh-my-zsh/ && \
    curl -L http://install.ohmyz.sh > install.sh && \
    sh install.sh && \
    git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting && \
    git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
COPY .zshrc /root/.zshrc



# RUN git clone https://aur.archlinux.org/code-server.git && \
#     cd code-server && \
#     makepkg -si && \
#     systemctl enable --now code-server@$USER









