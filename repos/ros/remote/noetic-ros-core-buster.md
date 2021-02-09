## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:eb0b55f4908bb7d8f9877a4895e91315d558d6a549c04ad63efac6edbedea26c
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
$ docker pull ros@sha256:bdcc644cc5c3e12c676695cb33a1c16537cbdeecda3a0fe393662bfb2cfceb22
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.3 MB (244260575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb4bdb2b7e043bec6fc4c270888566a1eea99e606a339645187439985f446192`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:40:45 GMT
ADD file:78412ee35e3dc6fb5fdfce41eb05dd273ba1d49328ab327465639bfa4821aa51 in / 
# Tue, 09 Feb 2021 02:40:50 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 17:56:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 17:56:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 09 Feb 2021 17:56:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 09 Feb 2021 17:56:19 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 17:56:20 GMT
ENV LC_ALL=C.UTF-8
# Tue, 09 Feb 2021 17:56:20 GMT
ENV ROS_DISTRO=noetic
# Tue, 09 Feb 2021 17:58:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 17:58:48 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 09 Feb 2021 17:58:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 09 Feb 2021 17:58:49 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c78c297fb0d010ee085f95ae439636ecb167b050c1acb4273bd576998cf94a83`  
		Last Modified: Tue, 09 Feb 2021 02:47:03 GMT  
		Size: 49.2 MB (49183229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7dc7e7c1a8c9728249478a065c8cbfb7b26a4ffcb6f0b8d2241f6af8e52bc0`  
		Last Modified: Tue, 09 Feb 2021 18:14:07 GMT  
		Size: 10.9 MB (10883298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94eec5caa2ce9024a59191b2c94308fe2f8cab9cea9031dc8de51fe09b658b9b`  
		Last Modified: Tue, 09 Feb 2021 18:14:05 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3affe42ffed8a74195454befbffcb5181f154b98092d214bc56ca825fc614162`  
		Last Modified: Tue, 09 Feb 2021 18:14:05 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569558cbdfd3b1304e6ccc1a802a2634583633f160a18c3e34ff32c204a1ae1a`  
		Last Modified: Tue, 09 Feb 2021 18:15:00 GMT  
		Size: 184.2 MB (184192209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eec434d09b660bdf210b479e8ab10f8dec24da00f6361f141deba874b5a5dd4`  
		Last Modified: Tue, 09 Feb 2021 18:14:05 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
