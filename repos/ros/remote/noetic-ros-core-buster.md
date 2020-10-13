## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:d18590a08c717d67b94cfdd232154fae6a2ad8c099524e79ea3e64cd6235cf32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:9c772bfd53fba9eab3a9d08b3d99a3f78eb55d57543a8d42ea52a9387269b785
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.2 MB (300152895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1949e62561ced5ee73027ad7415cb8b0f94cdccfbca2734e1c9c495e36f4dfe9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:30 GMT
ADD file:6627ad39ea0cb9fcb212342326d14efaff51aece1fd0dc16d5bbcaa25d858622 in / 
# Tue, 13 Oct 2020 01:38:30 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 19:24:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 19:24:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 13 Oct 2020 19:24:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 13 Oct 2020 19:24:03 GMT
ENV LANG=C.UTF-8
# Tue, 13 Oct 2020 19:24:04 GMT
ENV LC_ALL=C.UTF-8
# Tue, 13 Oct 2020 19:24:04 GMT
ENV ROS_DISTRO=noetic
# Tue, 13 Oct 2020 19:25:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 19:25:11 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 13 Oct 2020 19:25:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 13 Oct 2020 19:25:11 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e4c3d3e4f7b024979a1c12daa4073f6353b2ba92d96418bc90451994927c9bff`  
		Last Modified: Tue, 13 Oct 2020 01:48:02 GMT  
		Size: 50.4 MB (50395978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2a3a13f4da8a989cd47e5141fdd6f9cd9de6e86ccc396db6a668ad032a3160`  
		Last Modified: Tue, 13 Oct 2020 19:36:04 GMT  
		Size: 10.9 MB (10889343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64390ddd28a581349979be4bea66a21751b2ec96485b72280d0c7af425fbb8c`  
		Last Modified: Tue, 13 Oct 2020 19:36:02 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0caaf435d5f32518773b64abc379057bbd924c553cfeb58874f5b1315bfc735d`  
		Last Modified: Tue, 13 Oct 2020 19:36:02 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cfcaa897657f532536be04cfe0020d87bf81257a618757661653ce5441d295`  
		Last Modified: Tue, 13 Oct 2020 19:37:01 GMT  
		Size: 238.9 MB (238865739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14a3cb8bc6bc5df16b3677390c9b4780ea98a150b28e461422e141dbd5323b3`  
		Last Modified: Tue, 13 Oct 2020 19:36:02 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:95067f66d52b323aeeaf9f4223780b0d1581b68a24502edf90327703bcbfd3d8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.2 MB (244153769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a9495d40a9548226035103be73fffd9556c960dd462b730e867b475363500ea`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:40:40 GMT
ADD file:7a9016f6c75910c392bbea2cb9e146d1eba3942cdfd666a44004c79951c5d46f in / 
# Tue, 13 Oct 2020 01:40:45 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 20:39:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 20:40:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 13 Oct 2020 20:40:35 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 13 Oct 2020 20:40:45 GMT
ENV LANG=C.UTF-8
# Tue, 13 Oct 2020 20:40:50 GMT
ENV LC_ALL=C.UTF-8
# Tue, 13 Oct 2020 20:40:53 GMT
ENV ROS_DISTRO=noetic
# Tue, 13 Oct 2020 20:44:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 20:44:15 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 13 Oct 2020 20:44:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 13 Oct 2020 20:44:18 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:04aacb10cb67f5fa248646a0ac9f40af5a6d3b0dbef65505bb7766bed6bf4885`  
		Last Modified: Tue, 13 Oct 2020 01:47:53 GMT  
		Size: 49.2 MB (49175405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131ffa15211d55c8de67be0d0ced3bbec2336b0250efc1e38a00b49df2b3ca22`  
		Last Modified: Tue, 13 Oct 2020 21:00:55 GMT  
		Size: 10.9 MB (10882041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:946d470d5c44bd77a586608e501b75657edddef399cabbb3b784037a5b30de2c`  
		Last Modified: Tue, 13 Oct 2020 21:00:51 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3205eabe0fbcd56ebf5a0d111a79503bb9a68092500f018f21554bc69641b98e`  
		Last Modified: Tue, 13 Oct 2020 21:00:52 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a906801c61f426e1a99ed331e1f441f0731e34dee11c02124ef4c13b064b5c6`  
		Last Modified: Tue, 13 Oct 2020 21:01:56 GMT  
		Size: 184.1 MB (184094486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bbf60393679da03ef4644f7a560d3c43ca63dff47c5284f32bca35f7b2d7f4d`  
		Last Modified: Tue, 13 Oct 2020 21:00:52 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
