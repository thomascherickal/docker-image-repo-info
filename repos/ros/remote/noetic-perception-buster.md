## `ros:noetic-perception-buster`

```console
$ docker pull ros@sha256:38511c4b0a4043a53651d7039733d50b8bdafb294dc65f0c12a4f573080068c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-perception-buster` - linux; amd64

```console
$ docker pull ros@sha256:3dc735aa282843a7c175ab25a6ea9b650733d7e2586f796f9a507be73c13874b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **967.7 MB (967671794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57d4dfbca5e3c87961bf904b804cb2f63537410586fd5f0144c89f40789cae17`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:40 GMT
ADD file:8f75f11b2bd2d50e5912359ae750de06a7b49506df3756c19baf4cc63d900c4f in / 
# Tue, 09 Feb 2021 02:20:40 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 11:31:35 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 11:31:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 09 Feb 2021 11:31:38 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 09 Feb 2021 11:31:38 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 11:31:38 GMT
ENV LC_ALL=C.UTF-8
# Tue, 09 Feb 2021 11:31:39 GMT
ENV ROS_DISTRO=noetic
# Tue, 09 Feb 2021 11:33:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 11:33:14 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 09 Feb 2021 11:33:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 09 Feb 2021 11:33:15 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 11:34:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 11:34:11 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 09 Feb 2021 11:34:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 11:38:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0ecb575e629cd60aa802266a3bc6847dcf4073aa2a6d7d43f717dd61e7b90e0b`  
		Last Modified: Tue, 09 Feb 2021 02:26:22 GMT  
		Size: 50.4 MB (50400198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b0d5528d4d10129063ca7f720f24b759ff2414147dc9acb4ce80df4042a60c`  
		Last Modified: Tue, 09 Feb 2021 11:45:02 GMT  
		Size: 10.9 MB (10890381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fa6dc1339a6d69805730444ca620a9a352afd3a7004102f807586d106f5d23`  
		Last Modified: Tue, 09 Feb 2021 11:45:00 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6bbc1372440291fec04a189068eb2efaae76309c52126e7b243b4090f8b2bf0`  
		Last Modified: Tue, 09 Feb 2021 11:45:00 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c81b0773c3edd5e22f0d91661eb80b37b903b5c0d65fe00824b4414ed49690`  
		Last Modified: Tue, 09 Feb 2021 11:46:10 GMT  
		Size: 239.0 MB (238965006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb19dc30e7e64621f1fe2ec3c32280cf324c0e58cf772744426debd15fc3ae3`  
		Last Modified: Tue, 09 Feb 2021 11:45:00 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce894a3ca817b79ed4942f240675048b110277f1210e32393674430d7f89f88`  
		Last Modified: Tue, 09 Feb 2021 11:46:42 GMT  
		Size: 86.6 MB (86563808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0f0fb09c754a09ff6584dc9772046b55cc02e6d766bcf93f7a5c245b178153`  
		Last Modified: Tue, 09 Feb 2021 11:46:14 GMT  
		Size: 265.4 KB (265403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba79683d6e5abc56820da992383dcca1a9d7020af18307967bd372fd68c8237b`  
		Last Modified: Tue, 09 Feb 2021 11:46:43 GMT  
		Size: 76.0 MB (75966915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c1d0e58374e9de8bf242c89f61068e002f3f97252ba3f2f5dec053e8528756`  
		Last Modified: Tue, 09 Feb 2021 11:49:31 GMT  
		Size: 504.6 MB (504618246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:191eda2229c39afa1f511bcd4472805428bc1ad5923320fdbad6c56c7f166a0d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **884.5 MB (884503588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac074615d03366c82ce9b48d0eb1d8a943c58f1fbe30f3f3de5518fa01c20351`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:40:39 GMT
ADD file:849d424ecc8572facb3ca68eff836dce211bc677cb32d3c3eaa129d364d33878 in / 
# Tue, 12 Jan 2021 00:40:43 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 17:04:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 17:04:53 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 12 Jan 2021 17:04:56 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 12 Jan 2021 17:04:57 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 17:04:58 GMT
ENV LC_ALL=C.UTF-8
# Tue, 12 Jan 2021 17:04:59 GMT
ENV ROS_DISTRO=noetic
# Tue, 12 Jan 2021 17:07:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 17:07:22 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 12 Jan 2021 17:07:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 12 Jan 2021 17:07:24 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 17:08:12 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 17:08:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 12 Jan 2021 17:09:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 17:14:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e5587ff5efa4e647ae927194fac9b961a68d46b23b68a3119c90016e58f17aa`  
		Last Modified: Tue, 12 Jan 2021 00:51:18 GMT  
		Size: 49.2 MB (49183736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5133c142d67041b46437f81b1fad2248d916b31913015d0e9591ddd43e55a565`  
		Last Modified: Tue, 12 Jan 2021 17:23:32 GMT  
		Size: 10.9 MB (10882904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60827e914e9a578cc39153a996201569f0ac261afe2e8dd41b065ad0d72c9983`  
		Last Modified: Tue, 12 Jan 2021 17:23:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a4e1d21af11d75e8ff018a40f258e7cf9512d5bdf7a0b141113b7f039f1cb6`  
		Last Modified: Tue, 12 Jan 2021 17:23:29 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3812d77ac9cfc80389a8b87c3125fc82218e04f068455d0b4378af6503f7023c`  
		Last Modified: Tue, 12 Jan 2021 17:24:26 GMT  
		Size: 184.1 MB (184140147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f0e2a67e831045ba59fe86e0deda4aa5281459060f3c1b51a35b44db073eba`  
		Last Modified: Tue, 12 Jan 2021 17:23:29 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adfab3ab3df14a532c6a647e4bdd966155f097cb3bf1ddbaf99b3b510db8ab5`  
		Last Modified: Tue, 12 Jan 2021 17:24:50 GMT  
		Size: 84.4 MB (84353671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c980982f3d5f27708016f53ea3298c3838e5d5b387a2a044f0fd6e71bd5a23a2`  
		Last Modified: Tue, 12 Jan 2021 17:24:33 GMT  
		Size: 261.3 KB (261268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f2ea4eb5a9646660b14f96839384a2710939c0e33e1243f0ac2bda38b02108`  
		Last Modified: Tue, 12 Jan 2021 17:24:49 GMT  
		Size: 74.1 MB (74088325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a944688f9745d03cc36dade8a36836d3b3eeac699458d5a3ab9b6a6d7cb2387a`  
		Last Modified: Tue, 12 Jan 2021 17:27:24 GMT  
		Size: 481.6 MB (481591698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
