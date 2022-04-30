## `ros:foxy-ros-base`

```console
$ docker pull ros@sha256:4ffa1543fcac072dae1d2c20942d51e3c78c3af73c0fadd0e5825c91f2ba1c8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:a15b604fee96d0c4d7fcff2f6745cc909b917fd70f2231ceaf6b68eabdaa0fc3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.8 MB (251849799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1315244f74944de3809f9b5a1fbe724b88a727adba120da047be53586d22eb68`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:39:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:00:47 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:11:21 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 30 Apr 2022 02:11:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 30 Apr 2022 02:11:22 GMT
ENV LANG=C.UTF-8
# Sat, 30 Apr 2022 02:11:22 GMT
ENV LC_ALL=C.UTF-8
# Sat, 30 Apr 2022 02:11:22 GMT
ENV ROS_DISTRO=foxy
# Sat, 30 Apr 2022 02:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:12:24 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 30 Apr 2022 02:12:24 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 30 Apr 2022 02:12:24 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 02:12:55 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:13:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 30 Apr 2022 02:13:05 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 30 Apr 2022 02:13:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca43c78a9071a3a99b9aa1fe030cf8ba61c96fbf0b12adc1a85163d395cc10a1`  
		Last Modified: Sat, 30 Apr 2022 00:50:22 GMT  
		Size: 1.2 MB (1180884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695af473b1cd9e144d20d270ac7db7c1e34126fdb27db717ef1b82d4ea459397`  
		Last Modified: Sat, 30 Apr 2022 02:23:44 GMT  
		Size: 5.5 MB (5546712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ecbdd5d86aa1bccfbc93111261e6b9ae8bbd5777bcb704b395d81b82a8e6f7`  
		Last Modified: Sat, 30 Apr 2022 02:26:24 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184a755bf529bfea3fdd27ac8aa0a2c242d828fd03aa912766c514f925b0d324`  
		Last Modified: Sat, 30 Apr 2022 02:26:24 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c4352d7e2596c88ca8aa942219953143a17a9453871f288b5f352dbdb559f4d`  
		Last Modified: Sat, 30 Apr 2022 02:26:45 GMT  
		Size: 120.1 MB (120086250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea0e9bbed1d0b14dc544357de108d6f4ddafd24beb06a7734f5c47ba2142adbb`  
		Last Modified: Sat, 30 Apr 2022 02:26:25 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bf8fe277772f0499df386f672d466797d8e1b389cb7e27b531ed3f3bb91fdb`  
		Last Modified: Sat, 30 Apr 2022 02:27:06 GMT  
		Size: 74.5 MB (74540562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e4758ada805e565a51b082cf423dfcaa0584852447fc69f6389bb1e9c4400f`  
		Last Modified: Sat, 30 Apr 2022 02:26:55 GMT  
		Size: 254.9 KB (254921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a8c9291c7575bc8aceb707ad34ad1a467641e6cc4e996288462ad386f25d71`  
		Last Modified: Sat, 30 Apr 2022 02:26:55 GMT  
		Size: 2.2 KB (2192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7686189d3c32eaec4a6e9b36df3aaae350d4808eba51c1c14d374e463008add4`  
		Last Modified: Sat, 30 Apr 2022 02:26:58 GMT  
		Size: 21.7 MB (21669633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d7a58e5756d186f12b068619c563049cf692f41ad01230655a898c34094cb7f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.2 MB (227245810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b043bac584a9e6280aac004d04edc2f7fd3c65f9ebde897d71690ea1bd21216`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:20:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:20:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:25:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 30 Apr 2022 00:25:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 30 Apr 2022 00:25:53 GMT
ENV LANG=C.UTF-8
# Sat, 30 Apr 2022 00:25:54 GMT
ENV LC_ALL=C.UTF-8
# Sat, 30 Apr 2022 00:25:55 GMT
ENV ROS_DISTRO=foxy
# Sat, 30 Apr 2022 00:26:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:26:47 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 30 Apr 2022 00:26:48 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 30 Apr 2022 00:26:49 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:27:26 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:27:32 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 30 Apr 2022 00:27:37 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 30 Apr 2022 00:27:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2837428b54ca227343b28e2aebf5f943eb61317acb706203bbd53ccd36b1faa`  
		Last Modified: Sat, 30 Apr 2022 00:38:20 GMT  
		Size: 1.2 MB (1182149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782caaf301f52c6f48c207e662cbaff846f5e221ff2d301aa5123d59be9f9cdc`  
		Last Modified: Sat, 30 Apr 2022 00:38:18 GMT  
		Size: 5.3 MB (5321931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e518f0b96ea742e65f2524920ef0978594bec0e17d20b42b1068bfc73720bd`  
		Last Modified: Sat, 30 Apr 2022 00:41:03 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be28b19174686f17ae1317ae4d3c9000a0c5da2daba3797916241b4eff9b024e`  
		Last Modified: Sat, 30 Apr 2022 00:41:03 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e954138377bd97441a0963808a8c70e6c51bf87155d6bdb671530efd4a2af527`  
		Last Modified: Sat, 30 Apr 2022 00:41:20 GMT  
		Size: 104.3 MB (104266243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91245cadd2f0a13ba1496609e0e2f0f4b18302e97d37290d08553b24b77ad13`  
		Last Modified: Sat, 30 Apr 2022 00:41:02 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60afb6ca72387ba9902306d593fa053a9f27a64edd9dac6ed60164bd6606bc70`  
		Last Modified: Sat, 30 Apr 2022 00:41:42 GMT  
		Size: 68.7 MB (68673212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d22cef684130e343bfe87220672bc69f71f542aee8adce35eb893f194b2107b`  
		Last Modified: Sat, 30 Apr 2022 00:41:32 GMT  
		Size: 254.9 KB (254867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf97d0af157d8836375c4d09c7145909aa0c3043f4011e862c55162dbb4101a`  
		Last Modified: Sat, 30 Apr 2022 00:41:32 GMT  
		Size: 2.2 KB (2160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e657dd15b5ed4ccfe5d24e8cab5e2b032fe73c6e2edd134d2610969e5c8dc2a`  
		Last Modified: Sat, 30 Apr 2022 00:41:35 GMT  
		Size: 20.4 MB (20373496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
