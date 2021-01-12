## `ros:melodic-robot-stretch`

```console
$ docker pull ros@sha256:74e403280248998ae020bbbc76b1a31fcc6568b57326d727ee012bec4830c5a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-robot-stretch` - linux; amd64

```console
$ docker pull ros@sha256:60808a56ee9c96024369a639c990934188e69d37f879f4c06fbd884a7a1f5969
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **462.8 MB (462815251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdb39e55d6f51ea2ed380c5f3840e4ff647d523aa3c56c28d1a75272f75c5d13`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:35:05 GMT
ADD file:166cd044a29ad501c753917f07d638932f2ce960a8570b12d9155e8c38d1e917 in / 
# Tue, 12 Jan 2021 00:35:06 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:02:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:02:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 12 Jan 2021 01:02:50 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 12 Jan 2021 01:02:50 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 01:02:51 GMT
ENV LC_ALL=C.UTF-8
# Tue, 12 Jan 2021 01:02:51 GMT
ENV ROS_DISTRO=melodic
# Tue, 12 Jan 2021 01:04:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:04:24 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 12 Jan 2021 01:04:25 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 12 Jan 2021 01:04:25 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:05:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:05:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 12 Jan 2021 01:05:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:06:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2587235a7635c6991dfee9791c7977ab29694cf73bc64c3c5a79097ca99364d1`  
		Last Modified: Tue, 12 Jan 2021 00:43:05 GMT  
		Size: 45.4 MB (45380014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc107b7888825e0d5853ecf389db5b2515fe6326c73985cf48a2ce01aad26f5`  
		Last Modified: Tue, 12 Jan 2021 01:19:52 GMT  
		Size: 6.9 MB (6867770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf6fe34e55ea6e017ffb666a3989f281d46efd2f8515fcc9731d7c7bc9a5584`  
		Last Modified: Tue, 12 Jan 2021 01:19:52 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2572de55c9fd89fcf7d45082824b8a3847f1b721aa9cf9be7ed74f9dce36c0ff`  
		Last Modified: Tue, 12 Jan 2021 01:19:52 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75953d4f06b47b6e647839b21436c9ec886e57d4a9c6b2a49ca984ead018cccc`  
		Last Modified: Tue, 12 Jan 2021 01:21:07 GMT  
		Size: 270.0 MB (269996440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534164b2c2d43871e0b1a96ffe3f39b0af254e4d847fb1557cabcca5440b71b5`  
		Last Modified: Tue, 12 Jan 2021 01:19:53 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf6ad1cd65e8c47f1241487b6bcc2688fa67e744aaf3095c17e742ff36ea462`  
		Last Modified: Tue, 12 Jan 2021 01:21:43 GMT  
		Size: 70.2 MB (70152137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd5acb068dd42d818d372fd435d3f186e11db38dbc8430c80ee177a3bf3e6fc`  
		Last Modified: Tue, 12 Jan 2021 01:21:14 GMT  
		Size: 243.8 KB (243822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6369f3ff951a6a2e89d0fe30f2622871bd14906af898577a8555f3bea22f111a`  
		Last Modified: Tue, 12 Jan 2021 01:21:40 GMT  
		Size: 55.1 MB (55053482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6682bd58f34d51f668b7e726b02ddd33bf91a56b7a4d33a87c9d29c8d19fc5a`  
		Last Modified: Tue, 12 Jan 2021 01:21:56 GMT  
		Size: 15.1 MB (15119768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d2f57db8abd970382da3ce1028d293d6598a89a8471a74aba2857a0cf20a2fe1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **407.7 MB (407702576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:136011e281436c51e885c744040159a9ca20df447ed566ae9fa353a379999a7c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:48:16 GMT
ADD file:48e44714f486662ed380343e556f0f7411bd6600d916440063753c55d1f94b45 in / 
# Fri, 11 Dec 2020 02:48:17 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 23:10:51 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 23:10:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 11 Dec 2020 23:11:00 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 11 Dec 2020 23:11:01 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 23:11:02 GMT
ENV LC_ALL=C.UTF-8
# Fri, 11 Dec 2020 23:11:03 GMT
ENV ROS_DISTRO=melodic
# Fri, 11 Dec 2020 23:15:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 23:15:16 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 11 Dec 2020 23:15:17 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 11 Dec 2020 23:15:17 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 23:15:56 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 23:16:12 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 11 Dec 2020 23:17:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 23:17:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ecefb91918e846819df74a1beb8e41f454bef156738373818c20656a3a46d5f7`  
		Last Modified: Fri, 11 Dec 2020 02:55:36 GMT  
		Size: 43.2 MB (43175941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb876718fddc5fac92d1cf4a1a2bba55b4f1ef8004b2d667fb9d61f8b9788d3`  
		Last Modified: Fri, 11 Dec 2020 23:37:37 GMT  
		Size: 6.4 MB (6441718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d744afed63c33ced1159f376af8d52ad283a1081cdf38f545dcdd1b7b2331b7`  
		Last Modified: Fri, 11 Dec 2020 23:37:36 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb581dd072ca6ecb78ffb662d2eb6c37aac66cef0d6eb4a3598d85675b1f218`  
		Last Modified: Fri, 11 Dec 2020 23:37:36 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65fb0f9af0364eff78bd142ce79a274b31fdcb45ce2fee39fefe0b63bb868f61`  
		Last Modified: Fri, 11 Dec 2020 23:38:39 GMT  
		Size: 225.1 MB (225084656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b874e7e9fc0fdc699fa304738e4c71a8de8852a4e5e09810fd59a1b668de931c`  
		Last Modified: Fri, 11 Dec 2020 23:37:36 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84212fbdf8c4a6d26b8ff23a1a300a89abdc6ff29c1b96c9ee83e9d8651582df`  
		Last Modified: Fri, 11 Dec 2020 23:39:02 GMT  
		Size: 64.8 MB (64841404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f151d65d72e696d7d84bdf8e387141667efa44863d339afb7c216a3ccfdd1b`  
		Last Modified: Fri, 11 Dec 2020 23:38:46 GMT  
		Size: 242.0 KB (241988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d9e06feee4e4b021722a71a260bf00d8fee2bc210efa09939d06c086266d40c`  
		Last Modified: Fri, 11 Dec 2020 23:38:59 GMT  
		Size: 53.2 MB (53242246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba61288b7aff8b12769c061691d78b3be8de06c5622698154a5beb85267ca6fb`  
		Last Modified: Fri, 11 Dec 2020 23:39:13 GMT  
		Size: 14.7 MB (14672803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
