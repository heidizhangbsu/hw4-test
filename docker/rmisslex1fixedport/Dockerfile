FROM fedora
RUN  dnf -y install net-tools git java java-devel make
WORKDIR /home
RUN  (cd /home; git clone https://github.com/heidizhangbsu/hw4-test.git)
RUN (cd /home/hw4-test/docker/rmisslex1fixedport; javac *.java)
RUN /usr/sbin/ifconfig
CMD (cd /home/hw4-test/docker/rmisslex1fixedport; java DateServerImpl 5111)
