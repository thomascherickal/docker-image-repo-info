## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:5d21e8689227910f374250f55aaa6a7a8678fb7725448673e1fa200c5a31705a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:f3dbe3cf1f0e1d2c2b0adb8ddac8df3f590b1ed527e2bdc6d8188c2de1b9c825
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.3 MB (300257422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ded67ba18900fdb11442085664acf8ac510afa924099266ad757740d3016ac03`
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

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:e6aebb35f988188c6bd95049efecf3842bc2d43309f59f28ac27f24139616bbd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.2 MB (244208626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:585b53a99311e6884abce2e3c53a2b5aea71a813085995c58fd30cc869ff9bc8`
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
