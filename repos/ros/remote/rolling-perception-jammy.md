## `ros:rolling-perception-jammy`

```console
$ docker pull ros@sha256:a7e40cf9710295d15cb9b766b6f868ab2797b6b48b2e7edd4dd4730b957f1934
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `ros:rolling-perception-jammy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d965f32cbe5aece12862661161fd338c8674f438a8bbfc9b5a380249b7699109
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 GB (1036588183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6157fd95986698ac4e1e7f29cbd202c734ae8f00c288029494abaeeef44694f9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:52 GMT
ADD file:1e18e22e32f06a7e93275cf3a2eb2a1d3892be27628bdae2de4b2aadb992bd50 in / 
# Fri, 29 Apr 2022 22:49:53 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:32:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:32:26 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:32:26 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 30 Apr 2022 00:32:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 30 Apr 2022 00:32:29 GMT
ENV LANG=C.UTF-8
# Sat, 30 Apr 2022 00:32:30 GMT
ENV LC_ALL=C.UTF-8
# Sat, 30 Apr 2022 00:32:31 GMT
ENV ROS_DISTRO=rolling
# Fri, 27 May 2022 00:01:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 27 May 2022 00:01:50 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Fri, 27 May 2022 00:01:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 27 May 2022 00:01:52 GMT
CMD ["bash"]
# Fri, 27 May 2022 00:02:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 27 May 2022 00:02:37 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 27 May 2022 00:02:41 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 27 May 2022 00:03:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 27 May 2022 00:06:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-perception=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b84950154c181a602d2e93b68e84660f96dc78f94ae36f3df2db8d5701abb6a5`  
		Last Modified: Fri, 29 Apr 2022 22:52:07 GMT  
		Size: 28.4 MB (28376457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4339dcf07e4fd919aa10dc0e01fb8f44184f74bf6baf5aef6e8fdd30f5e603`  
		Last Modified: Sat, 30 Apr 2022 00:43:58 GMT  
		Size: 1.2 MB (1192681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0db3fdf5b04e561797500fc1d19d79a37ca0586b71bee71ce2acaee153d4dee`  
		Last Modified: Sat, 30 Apr 2022 00:43:56 GMT  
		Size: 3.6 MB (3594435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13af71d8cd404a31e077722270696cf33d59cff54d35c9dad864264138bc3ac`  
		Last Modified: Sat, 30 Apr 2022 00:43:55 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19e01b1250d40bc108a995e5fc6c1630b0abdbfff31529a87a4096271f2a6115`  
		Last Modified: Sat, 30 Apr 2022 00:43:55 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb42783cc3927279718097f695acb188af7247f4635771cc2e94fd788d4b0118`  
		Last Modified: Fri, 27 May 2022 00:10:41 GMT  
		Size: 106.4 MB (106386146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c9f41ded8565c1f327636498d36859881d62a32bdc9dff5b92e047d59012dd`  
		Last Modified: Fri, 27 May 2022 00:10:24 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91de34af377d115902131c5b5ca87d21c9fffb69370e16847717d2e1a2a40bd4`  
		Last Modified: Fri, 27 May 2022 00:11:07 GMT  
		Size: 95.2 MB (95224066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731ff29b8d2944a451a664aa964b37ab3dae63c3ea232467461df0af1282e4e8`  
		Last Modified: Fri, 27 May 2022 00:10:53 GMT  
		Size: 271.5 KB (271498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379ba5086e791ab84c3886a744c998db4d34535d380f06dea5be896569e00b76`  
		Last Modified: Fri, 27 May 2022 00:10:53 GMT  
		Size: 2.2 KB (2175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736e7996fb31e59ebb99c1d6d574b039f8d52c9d6e1e6a665c4f3e7ca7ff604d`  
		Last Modified: Fri, 27 May 2022 00:10:57 GMT  
		Size: 22.4 MB (22444755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c670e91d82a9ed28fffade82b8bf56c937e32ac2de425c79b22d3068855572c`  
		Last Modified: Fri, 27 May 2022 00:12:56 GMT  
		Size: 779.1 MB (779093601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
