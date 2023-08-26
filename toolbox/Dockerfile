FROM registry.fedoraproject.org/fedora-toolbox:latest

# Install extra packages
COPY pkgs /
RUN dnf -y update --refresh
RUN dnf -y install $(<pkgs)
RUN rm /pkgs
