
# Pull base image.
FROM fagorautomation/ubuntu-base

# Ubuntu Yocto dependencies (Mega Manual):
# Essentials
RUN sudo apt-get install -y gawk wget git-core diffstat unzip texinfo gcc-multilib \
build-essential chrpath socat cpio python python3 python3-pip python3-pexpect \
xz-utils debianutils iputils-ping

# Graphical and Eclipse Plugin Extras
RUN sudo apt-get install -y libsdl1.2-dev xterm

# Documentation
RUN sudo apt-get install -y make xsltproc dockbook-utils fop dblatex xmlto

# OpenEmbedded Self-Test
RUN sudo apt-get install -y python-git

# kernel compilation rpi needs this
RUN sudo apt-get install -y bc libncursesw5-dev

# Use baseimage-docker's init system.
CMD ["/sbin/my_init"]
