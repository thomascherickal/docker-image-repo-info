## `ros:rolling-ros-core`

```console
$ docker pull ros@sha256:0e7875d1f332c025ea2471dda47bc26e6b92ac8745391ba55f34fb877040b470
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:cc56027496019e29cb7f8c3c52c13533ab161b783d9f21986968cbe449d5d0c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.8 MB (151849868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03e81171fdda7aceab141fe9243b1e1b064fab7d1ebe5f238ef7fdb2fcdd16e9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:31:09 GMT
ADD file:ce9bee138da151fa0b9e441f7ef06865e0171006e686f0dc5e1ca6a06e0a3d0c in / 
# Fri, 18 Mar 2022 05:31:09 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:53:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:53:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:53:42 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 09:54:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:54:18 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:54:18 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:54:18 GMT
ENV ROS_DISTRO=rolling
# Fri, 18 Mar 2022 09:56:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:56:20 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 09:56:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:56:20 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:11581404396c9d08d16b97c64bb2fd043ef3216bd3e3ff3d1c6e03398dc8e336`  
		Last Modified: Wed, 16 Mar 2022 11:30:57 GMT  
		Size: 30.5 MB (30485551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36d449d4c1f6f849759c38658c4e2053c7b2950c7f69d42c0fcdbd7fd490b7d`  
		Last Modified: Fri, 18 Mar 2022 10:11:05 GMT  
		Size: 1.2 MB (1192034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855467c60b27cd7745629db97415c3b46e1b14929c08528fe5e29366df56502c`  
		Last Modified: Fri, 18 Mar 2022 10:11:03 GMT  
		Size: 3.8 MB (3826992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f6ac5bb5e9af926be15f77146a24734345444a1a6adaff26e3e6294242a743`  
		Last Modified: Fri, 18 Mar 2022 10:11:02 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4282676e74b396a8e1c48a6889a965866ac0fb68c719a00711200bd53e3e198`  
		Last Modified: Fri, 18 Mar 2022 10:11:02 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3605b0dd24d9612e9bf001c434a312571f6c91a4e4195d8fb584835cbdd08c`  
		Last Modified: Fri, 18 Mar 2022 10:11:27 GMT  
		Size: 116.3 MB (116342876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47eb45f708718a35b2c6e268082dd402aa16bdd526b8281bbb3516dd9ea94dd`  
		Last Modified: Fri, 18 Mar 2022 10:11:02 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:33fb547172debbc26b8b51c53c0093dd61aa633905cd5c25497ebd7e3c174669
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.2 MB (149222924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a8825532c46ae89a067cb23a4e016b986c597c0733c3bf539051d86d723235d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:41:10 GMT
ADD file:c81be95ae491788086dc606dd86ac47b679f2ce48c96016d4ba321e995541bca in / 
# Fri, 18 Mar 2022 00:41:11 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 01:14:40 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:14:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:14:51 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 18 Mar 2022 01:15:24 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 01:15:25 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 01:15:26 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 01:15:27 GMT
ENV ROS_DISTRO=rolling
# Fri, 18 Mar 2022 01:16:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 01:16:20 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 18 Mar 2022 01:16:21 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 01:16:22 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:8037d5c930bd3f2cc0b5ef6849e32124c3c5efaf4389d0974934bba554464390`  
		Last Modified: Fri, 18 Mar 2022 00:43:17 GMT  
		Size: 28.4 MB (28425528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52a2d6d51d5672d6a89bcd061ceb0abb70543ab14cf758b52dae0ea10a9ed89`  
		Last Modified: Fri, 18 Mar 2022 01:29:49 GMT  
		Size: 1.2 MB (1193964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a484c953b5a8ac5a49bdfa6ef2654513ce04b2c545724ed23887ed4e26ecf1e0`  
		Last Modified: Fri, 18 Mar 2022 01:29:46 GMT  
		Size: 3.6 MB (3594382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c71cdbe64ce9e2a57214b4db9fcdfb68ece3c8c4d618cd6e7ca840103a663f3`  
		Last Modified: Fri, 18 Mar 2022 01:29:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff9291a332798080bfb5b2e8ffa0d988a72c8939ca254eb21592d43f1716372`  
		Last Modified: Fri, 18 Mar 2022 01:29:46 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b90c99c3d8313d7660084c587776cc644ff55ca2453c2b9abd86d7d6236df1`  
		Last Modified: Fri, 18 Mar 2022 01:30:05 GMT  
		Size: 116.0 MB (116006679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:124e2c942e9e5613f749e090c5d6e24e6309980924397b270887cdec8ef21a9a`  
		Last Modified: Fri, 18 Mar 2022 01:29:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
