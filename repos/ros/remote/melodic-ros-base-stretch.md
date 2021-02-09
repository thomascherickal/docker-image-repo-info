## `ros:melodic-ros-base-stretch`

```console
$ docker pull ros@sha256:327c3ebfba147c1ae662e8968dd26d466b9736efc114db2b5e7a168607490ddd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-stretch` - linux; amd64

```console
$ docker pull ros@sha256:004a25d5ca75f9ed2690166c9865d009a029f496c4b234cac242a7e716716ba1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **447.7 MB (447700873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3da763bb42811750b61a8adfdd8fac6ed27d07eae69458316dfe39bb5dc63830`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:23:13 GMT
ADD file:e1e13145e23f170f2d55444019a2d18a8cecd6209bba9f4295a35632ad53fdde in / 
# Tue, 09 Feb 2021 02:23:14 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 11:24:08 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 11:24:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 09 Feb 2021 11:24:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 09 Feb 2021 11:24:15 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 11:24:15 GMT
ENV LC_ALL=C.UTF-8
# Tue, 09 Feb 2021 11:24:16 GMT
ENV ROS_DISTRO=melodic
# Tue, 09 Feb 2021 11:26:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 11:26:09 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 09 Feb 2021 11:26:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 09 Feb 2021 11:26:09 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 11:26:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 11:27:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 09 Feb 2021 11:27:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1e987daa2432270bbfaf366f57583c93b48e0ee6c9fe54fe7f4030b84095627f`  
		Last Modified: Tue, 09 Feb 2021 02:29:20 GMT  
		Size: 45.4 MB (45379885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dfef8404fefc17dca87eada52dd07e7bf488497c0c31fea11a60d978da694ad`  
		Last Modified: Tue, 09 Feb 2021 11:41:05 GMT  
		Size: 6.9 MB (6868182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c6e767fccda9923a28109011a5e7fdda7e9f5841c99cc59bee58d437744ceaa`  
		Last Modified: Tue, 09 Feb 2021 11:41:03 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973024f9f826542d72aca896bca3ed1f99093289ca8442460a1d25549bed8bcd`  
		Last Modified: Tue, 09 Feb 2021 11:41:04 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a0b85ea3938d10333f243bfd23c5bed7f06b58b3a5aaaeca4007a5e2b2eb84`  
		Last Modified: Tue, 09 Feb 2021 11:42:10 GMT  
		Size: 270.0 MB (269998323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f36fe789310fd477065fed5386f3d7ac24047a56072617d59131f960a643d88`  
		Last Modified: Tue, 09 Feb 2021 11:41:03 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c74144c81a256f811ce993305c224a0dbe9432e6de9707d6362cc46160e2a20`  
		Last Modified: Tue, 09 Feb 2021 11:42:51 GMT  
		Size: 70.2 MB (70152536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89db447f03061cc7b020dab71976df77709f2668c750794810919c0d7494d6d3`  
		Last Modified: Tue, 09 Feb 2021 11:42:15 GMT  
		Size: 246.4 KB (246447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca203fed66a213b3b04ebec6a1c62c6c7ee68c202941aa3289672514f40906c7`  
		Last Modified: Tue, 09 Feb 2021 11:42:39 GMT  
		Size: 55.1 MB (55053684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:b3753763f993b1af24cb03698c3a1e4488ca30fe2cded3ae25e306dff5a5b983
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **393.1 MB (393051724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5562ecd37893b7155564b1b8cc3bd0277e3093b83675a60246930d5c30a3cf7b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:43:17 GMT
ADD file:fb69ff7b2a28f793efbd16e04b74ffb4557d39e1844b3789075b4d3ff97a0eaa in / 
# Tue, 09 Feb 2021 02:43:20 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 17:45:04 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 17:45:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 09 Feb 2021 17:45:14 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 09 Feb 2021 17:45:16 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 17:45:17 GMT
ENV LC_ALL=C.UTF-8
# Tue, 09 Feb 2021 17:45:18 GMT
ENV ROS_DISTRO=melodic
# Tue, 09 Feb 2021 17:47:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 17:48:01 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 09 Feb 2021 17:48:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 09 Feb 2021 17:48:03 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 17:48:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 17:49:07 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 09 Feb 2021 17:50:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:296c9f0bf5f2cf24e87bc5abd674fc486e8df419d4aa2d362453f64d38900504`  
		Last Modified: Tue, 09 Feb 2021 02:49:43 GMT  
		Size: 43.2 MB (43177550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ade37f2522e7128b3ea67c5d6305b85511d46b9e28ea64de5aa7a7d73fde2e3`  
		Last Modified: Tue, 09 Feb 2021 18:10:34 GMT  
		Size: 6.4 MB (6442794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d691ed68a96a9727b6f7d8dae921417288b01b55a27d62ce784af530053a588c`  
		Last Modified: Tue, 09 Feb 2021 18:10:32 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4030e2d7bc052a230c7a0b5c1e1a8dcea8cc2c963bd1d9ba797fe7279f393473`  
		Last Modified: Tue, 09 Feb 2021 18:10:31 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8227e2dbefe02c9376f459ec37b8cfe86c3d8bc01f9f8bdf8607f1b5bca9a494`  
		Last Modified: Tue, 09 Feb 2021 18:11:36 GMT  
		Size: 225.1 MB (225098504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5954db5c24670b97e935da3e333d21ac12d20fb2bff2604bcb09456ae5ca3e`  
		Last Modified: Tue, 09 Feb 2021 18:10:32 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c566f755da002a1419c1b1c3b09b021387896822e6350bb89436933cfc1b1a1`  
		Last Modified: Tue, 09 Feb 2021 18:11:59 GMT  
		Size: 64.8 MB (64841293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0bc8f7336419b5dd77761d3f5dee5ec06bfe954590208490394ad60a87da10`  
		Last Modified: Tue, 09 Feb 2021 18:11:42 GMT  
		Size: 246.5 KB (246499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:049093b6de69735edfcb63e4dab9458cf042741a6f57cdbc5eba8be61a75da53`  
		Last Modified: Tue, 09 Feb 2021 18:11:55 GMT  
		Size: 53.2 MB (53243267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
