# Centos Load
Bootstrap: yum
OSVersion: 7
MirrorURL: http://mirror.centos.org/centos-%{OSVERSION}/%{OSVERSION}/os/$basearch/
Include: yum


# Generic Load
#Bootstrap:docker
#From:ubuntu:latest  

%help
#################################
Thank you for download the OPPNI container.
No other help is availible.
help		help command plaintext
setup		bash commands to set up the system
files		a host and image image drop into the container, plain text
labels		tidbits of information for storage
environment	adding enviro variables and exporting for runtime, like bash_profile
post		inside container - installing, making and downloading
runscript	singularist run X, can get arg flags via $*
test		testing after the end of the build

%setup
#################################
# Run code on the host
	echo "Preforming Setup like .bash_profile would"

	echo "This is the root, copy files to here not using it will be outside the image"
#touch ${SINGULARITY_ROOTFS}/tacos.txt
#touch avocados.txt

	echo $SINGULARITY_ROOTFS

	echo "Looking for existing OPPNI paths"
	echo $AFNI_PATH
	echo $FSL_PATH 
	echo $OPPNI_PATH


%files
	

%labels
	Maintainer AndrewLofts
	Version v1.0


%environment
##################################
# Set Up environment Here
#RAWR_BASE=/code
#export RAWR_BASE




#exports

  
%post  
##################################
	echo preping host enivronment before image runs



%runscript
##################################
# This is the main section of code that is activated
# This is what will interact with the oppni shell
	echo "Running OPPNI" 
#exec /bin/bash /code/rawr.sh "$@"

%test
##################################
# Custom Tests to confirm the script is successful
