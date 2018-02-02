Bootstrap: docker
From: centos:6.9

%environment
    LD_LIBRARY_PATH=/mnt/abc/u/staff/hwleong/craylibs:$LD_LIBRARY_PATH
    export LD_LIBRARY_PATH
    PATH=/mnt/abc/u/staff/hwleong/test/singularity/openmpi-2.1.0/bin:$PATH
    export PATH
    
%help
My test image for centos 6.9. Author: hwleong

%labels
Author: Hon Wai, Leong

%post
    echo "Installing Development tools"
    yum -y groupinstall "Development Tools"
    echo "Installing other utilities"
    yum -y install wget tcl
    echo /mnt/abc/u/staff/hwleong/craylibs >> /etc/ld.so.conf

