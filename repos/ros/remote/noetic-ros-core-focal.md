## `ros:noetic-ros-core-focal`

```console
$ docker pull ros@sha256:b8217be1fc3e6b6ff050a3240c45a7b22afc4b666ba37be64b663dc015742f34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-focal` - linux; amd64

```console
$ docker pull ros@sha256:6c08c842014ab47086b7c7cf44822c1c38eb29021e3a507dd15f96c91bd80ef7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.0 MB (212000331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34ca8509b2bc392cc43532c37d24093e0f2f9a034d86a6fca08aba57f40c5d59`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:03:08 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:02:13 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 06:02:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 06:02:23 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 06:02:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 06:02:23 GMT
ENV ROS_DISTRO=noetic
# Fri, 01 Oct 2021 06:04:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:04:15 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 06:04:15 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 06:04:15 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6d2c6667ea5660473b4dbbded093f5fb0330bb09072dd5f023fe8917898f5`  
		Last Modified: Fri, 01 Oct 2021 05:15:23 GMT  
		Size: 1.2 MB (1183161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d76f6f81fcfbb67046fda7409d7f51373035330bf4b0b3f29d51ce1531379df`  
		Last Modified: Fri, 01 Oct 2021 06:24:29 GMT  
		Size: 5.5 MB (5547583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8985568900a589503a6b64505536a7ed14c04be58f49125487546556e4bf16d2`  
		Last Modified: Fri, 01 Oct 2021 06:24:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d396a66dc135f942aded0cbf41869920dd471f4ae69a577ef485c7fad6ad26f6`  
		Last Modified: Fri, 01 Oct 2021 06:24:28 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0e67a2d329fca5d4ed9676dc99b6786e3b630fb2cdc61a582593ee9c0d2af6`  
		Last Modified: Fri, 01 Oct 2021 06:24:57 GMT  
		Size: 176.7 MB (176698260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14f46e6b695aaf67ea964cbc89cec1bb208303e42ef77d8ae91776e089bb5ca`  
		Last Modified: Fri, 01 Oct 2021 06:24:28 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:16e7b5ad0816dfb995956431231354e9108fc4bf112b8837081c4df3804bfec7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.1 MB (187147799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71a616ba0d071ae4bd5b86fb577470a9d32a66c3c8fb9b569bfc03c1149ac6dc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:52 GMT
ADD file:f9dcf17ef0f45719dff5ed961907d78a1ea6671fecdb434536f3fc8cf15fbb3b in / 
# Tue, 31 Aug 2021 01:40:53 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:58:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:58:31 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:58:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Aug 2021 03:58:39 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Aug 2021 03:58:40 GMT
ENV LANG=C.UTF-8
# Tue, 31 Aug 2021 03:58:40 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Aug 2021 03:58:40 GMT
ENV ROS_DISTRO=noetic
# Tue, 31 Aug 2021 04:01:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 04:01:06 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 31 Aug 2021 04:01:06 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Aug 2021 04:01:07 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:cccc98128e2b3db00394b4e59c3f674a52e4b861786d9fab388357a88fc428a2`  
		Last Modified: Tue, 31 Aug 2021 01:44:57 GMT  
		Size: 24.1 MB (24068823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3597f16c1171caedee0148b09aba1a7c8b8ff2f29ffec5f8bc82f4a2d0c4a955`  
		Last Modified: Tue, 31 Aug 2021 04:17:31 GMT  
		Size: 1.2 MB (1183503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503f278f986afdfeaabcdd6e3e66554d2851e9813dda91fc83341f7cdf3dca05`  
		Last Modified: Tue, 31 Aug 2021 04:17:30 GMT  
		Size: 4.7 MB (4676468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf026e89b16b8250a76b892191540bf0879aafa7e00242a2f6151d466ee9f283`  
		Last Modified: Tue, 31 Aug 2021 04:17:27 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2c21ec0037b0f9bae7c4c1a4415d768ebce97dc86e798bff4f6e544059ac5e`  
		Last Modified: Tue, 31 Aug 2021 04:17:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db678ae234a6fe1d46c8463a559f04c415c2522d0effab08ae407178410d5db`  
		Last Modified: Tue, 31 Aug 2021 04:19:33 GMT  
		Size: 157.2 MB (157216591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79678cecea953d0568fb159f017c76dd5db59346cc095d3d118b734bade1037d`  
		Last Modified: Tue, 31 Aug 2021 04:17:27 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:6facbfe8fce44d9ee05d3b498a246e9f803369ec0409cca79b8317d52ff417be
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.0 MB (205007074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1316784178101ce1bbeecbf3774b544a6e8e8741e4a498bccbae95017b7c74b4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:05:21 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 04:05:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:05:34 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:05:34 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:05:34 GMT
ENV ROS_DISTRO=noetic
# Fri, 01 Oct 2021 04:06:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:06:24 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 04:06:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:06:24 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca36dcb5509e6b267d7d917bd37bab3a2fe9b3bb7fc75f0ac08d43124d65dcaa`  
		Last Modified: Fri, 01 Oct 2021 04:21:14 GMT  
		Size: 1.2 MB (1183644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a8b61bc4869c8fd71f74e111385e4330a1f33dc9a4e9479a0721d070693113`  
		Last Modified: Fri, 01 Oct 2021 04:21:12 GMT  
		Size: 5.5 MB (5512866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5955ec7390235db14b9c45d9030bd90295fdbfc2dd976b408668c1feaa0c16ba`  
		Last Modified: Fri, 01 Oct 2021 04:21:11 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3177f1eddf2202fb915200162e8693b4fc55482d73411891f1184df5517140`  
		Last Modified: Fri, 01 Oct 2021 04:21:11 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76170f07a4a0b1a928e2367788be540ac8379fbb9cdd2461ef5248e67f7ffb96`  
		Last Modified: Fri, 01 Oct 2021 04:21:43 GMT  
		Size: 171.1 MB (171135747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002ffa5ef1c6b2f2640d24037747e349bcb1b99eaba29240f0b7e62c35115462`  
		Last Modified: Fri, 01 Oct 2021 04:21:11 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
