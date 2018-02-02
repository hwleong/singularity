Bootstrap: docker
From: centos:6.9

%help
My test image for centos 6.9. Author: hwleong

%labels
Author: Hon Wai, Leong

%post
    echo "Installing Development tools"
    yum -y groupinstall "Development Tools"
    echo "Installing other utilities"
    yum -y install wget tcl
    
%appenv mpi
    SCIF_APPBIN_mpi=/mnt/abc/u/staff/hwleong/singularity/openmpi-2.1.0/bin
    SCIF_APPLIB_mpi=/mnt/abc/u/staff/hwleong/singularity/openmpi-2.1.0/lib:/mnt/abc/u/staff/hwleong/craylibs
