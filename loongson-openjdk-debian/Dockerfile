FROM aoqi/debian-mips64el:stable

#RUN apt-get -qq update

# Install Loongson OpenJDDK 8
RUN cd /tmp && \
    wget -q "http://ftp.loongnix.org/toolchain/java/openjdk8/jdk8-mips64-8.tar.gz" && \
    tar xf jdk8-mips64-8.tar.gz -C /opt && \
    rm -f jdk8-mips64-8.tar.gz

# Define commonly used JAVA_HOME variable
# Add Loongson OpenJDK into PATH variable
ENV JAVA_HOME=/opt/j2sdk-image \
    PATH=${PATH}:/opt/j2sdk-image/bin
