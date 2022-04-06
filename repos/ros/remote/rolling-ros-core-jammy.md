## `ros:rolling-ros-core-jammy`

```console
$ docker pull ros@sha256:fc521098779f241e12f7ef08c938d8eebe03e4a7a3a028ae66512ebabf88ad1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-core-jammy` - linux; amd64

```console
$ docker pull ros@sha256:115d2319079b47894b46b3e9e62a408ee3b0bc26cf1000428ac9ee8927280fb5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141829904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed9fb867b97a7abb529f7ae53f0f4c614bbc22cf8915e8c526d5babad053d4a0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:21:07 GMT
ADD file:7c41c66243d4fb7f89ee02cc01d5befb32079e87dac32fb83e205e92b9acc0bc in / 
# Tue, 05 Apr 2022 22:21:07 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 02:38:37 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 02:38:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 02:38:54 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 06 Apr 2022 02:38:56 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 06 Apr 2022 02:38:56 GMT
ENV LANG=C.UTF-8
# Wed, 06 Apr 2022 02:38:56 GMT
ENV LC_ALL=C.UTF-8
# Wed, 06 Apr 2022 02:38:56 GMT
ENV ROS_DISTRO=rolling
# Wed, 06 Apr 2022 02:40:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 02:40:32 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 06 Apr 2022 02:40:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 06 Apr 2022 02:40:33 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:494bf829f3895588d3c99674907f92507f4f902e5e75871dca3149b95cdc86c7`  
		Last Modified: Tue, 05 Apr 2022 13:23:41 GMT  
		Size: 30.4 MB (30444702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e3acb8f9efe79e6809a90757c1f343f04d8504a0d8acd71ecf81355e123f3d9`  
		Last Modified: Wed, 06 Apr 2022 02:51:22 GMT  
		Size: 1.2 MB (1191458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f398145d9c235e43390420ac15d9bd36c93a8c451e727aca48a1eeb74b375c7c`  
		Last Modified: Wed, 06 Apr 2022 02:51:20 GMT  
		Size: 3.8 MB (3827038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:632e593d0e55a63e13eac91243ae8a895b0e7ae2b5b4eee50af0536b4190f8db`  
		Last Modified: Wed, 06 Apr 2022 02:51:19 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b3d5fb04541fd3046af1da67b0acf6e7a6cb2a1b2b55feeb31e54b9e6b13e1`  
		Last Modified: Wed, 06 Apr 2022 02:51:20 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925dedc957ba9dda5bf275258de20233e55b532ab457c6392b0a7a69764379d2`  
		Last Modified: Wed, 06 Apr 2022 02:51:36 GMT  
		Size: 106.4 MB (106364290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63060bdc53ba60da015b85c141d325483b19619ffdbafbc5d4215623e53f5ac7`  
		Last Modified: Wed, 06 Apr 2022 02:51:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-core-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9d5da515fe18d479f3314d4191972c75cebafd1dd6cb64ddd0bd15ca9082ecaf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137293435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:213be688526862e497ffef28fdf87f8602780db3780efd1372786bc906ac7bfb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:41:19 GMT
ADD file:49571aac1d9686cc3e1be327834e8e0a9d0cdef8501fe221dfa628689bd7459a in / 
# Tue, 05 Apr 2022 22:41:20 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 00:18:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:19:00 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:19:00 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 06 Apr 2022 00:19:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 06 Apr 2022 00:19:03 GMT
ENV LANG=C.UTF-8
# Wed, 06 Apr 2022 00:19:04 GMT
ENV LC_ALL=C.UTF-8
# Wed, 06 Apr 2022 00:19:05 GMT
ENV ROS_DISTRO=rolling
# Wed, 06 Apr 2022 00:19:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:19:53 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Wed, 06 Apr 2022 00:19:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 06 Apr 2022 00:19:55 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b267b9306c29bd8ae0bcc24ca28ea93e4424c701b94c4c0390bed799035db1c2`  
		Last Modified: Tue, 05 Apr 2022 13:24:30 GMT  
		Size: 28.4 MB (28399696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b17b1d14578e77e94554d5f4cf5d57031c592a57d5e141dd2e1f315bf22b507b`  
		Last Modified: Wed, 06 Apr 2022 00:30:24 GMT  
		Size: 1.2 MB (1192992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef948273a9607114de626af36a172cc0c15b08e2b942cc60ae398e7e571761e2`  
		Last Modified: Wed, 06 Apr 2022 00:30:22 GMT  
		Size: 3.6 MB (3594808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a0d2d283baed3854d5b74f3b1737ff1b6aebd7c95e7da4b6c77aa9cd351e6f6`  
		Last Modified: Wed, 06 Apr 2022 00:30:21 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a64369f63105fbe089b86048d1fe215afed2addd095de9e31a8f72df9a6a1d1`  
		Last Modified: Wed, 06 Apr 2022 00:30:21 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5adcc3bb85ed3dcb070e9a91ae8904c45ce1890de81416a01f7df032fc332ecf`  
		Last Modified: Wed, 06 Apr 2022 00:30:38 GMT  
		Size: 104.1 MB (104103567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd51021e46a98c41a88da0dab0e91b29d8a36fc74269a945b52b76ab590e5c9`  
		Last Modified: Wed, 06 Apr 2022 00:30:22 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
