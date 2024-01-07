FROM kalilinux/kali-rolling

RUN apt-get update && \
    apt-get install -y kali-desktop-xfce \
                       tightvncserver \
                       xfonts-base

RUN mkdir ~/.vnc
RUN echo "kali-docker" | vncpasswd -f > ~/.vnc/passwd
RUN chmod 600 ~/.vnc/passwd

EXPOSE 5901

CMD ["vncserver", ":1", "-geometry", "1280x800", "-depth", "16"]