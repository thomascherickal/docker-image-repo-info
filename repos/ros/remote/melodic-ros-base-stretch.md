## `ros:melodic-ros-base-stretch`

```console
$ docker pull ros@sha256:4be1b72117726a5c7b2af3b972b2de2369d4be75f77145581dc498be4f7e77aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-stretch` - linux; amd64

```console
$ docker pull ros@sha256:a5280ffe4b40f777153bb7b8f98f86451f61cc250543851e4dfa025e95b42eec
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **447.9 MB (447868009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33e6ba356d6580b1a9501b089ba6daa7ff4dfc61c0fa03d84870fae1d0fb7c25`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:20 GMT
ADD file:6e16bc9cf28c19a1fb1fb516411643e33cbd2bdb7b6c2ce2468c6583c89871a2 in / 
# Tue, 09 Jun 2020 01:23:21 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 20:24:20 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 20:24:24 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 09 Jun 2020 20:24:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 09 Jun 2020 20:24:26 GMT
ENV LANG=C.UTF-8
# Tue, 09 Jun 2020 20:24:26 GMT
ENV LC_ALL=C.UTF-8
# Tue, 09 Jun 2020 20:24:26 GMT
ENV ROS_DISTRO=melodic
# Tue, 09 Jun 2020 20:26:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 20:26:11 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 09 Jun 2020 20:26:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 09 Jun 2020 20:26:11 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 20:26:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 20:27:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 09 Jun 2020 20:27:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:81fc1918191541a2ffb6ed1cd8386ef8302aea1b0613ebc768a00e76c1f34bb9`  
		Last Modified: Tue, 09 Jun 2020 01:27:59 GMT  
		Size: 45.4 MB (45375796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e53c331f2ecda6ec4f9119258b0b88f1dc218bc1e67ba82cb01a51942b25544`  
		Last Modified: Tue, 09 Jun 2020 20:37:22 GMT  
		Size: 6.9 MB (6865099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f44dc7569baa1eebbc5e1f5560794048d8ba35421873de7531310f8082c0c7`  
		Last Modified: Tue, 09 Jun 2020 20:37:20 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948152c2814e825ed688e3a3048f639f0fb3eccef07021e0a0d6e15f3be182ea`  
		Last Modified: Tue, 09 Jun 2020 20:37:20 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b4136b73b353797b6cf84a63c456c39bb9485b7b1447f2c6616474dd330da2`  
		Last Modified: Tue, 09 Jun 2020 20:39:21 GMT  
		Size: 269.8 MB (269816794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651404712d7315cbd7e8cebf1f5c9b0d54a0c8b3d60974a39b80501691b64794`  
		Last Modified: Tue, 09 Jun 2020 20:37:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d3b6cbf0fdf31e283f61f59ab0047953dd7ed187b6b7ea72ca86684215939d9`  
		Last Modified: Tue, 09 Jun 2020 20:39:42 GMT  
		Size: 70.1 MB (70149728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc669c511abb5312e82b08cc6b6848c7264865d70e0f7ad9bb9c2932013d785`  
		Last Modified: Tue, 09 Jun 2020 20:39:26 GMT  
		Size: 249.2 KB (249211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c23826b3ac75e6b24b78d96ecd254196ae239cbf2b8180c56916a1fbd439af0`  
		Last Modified: Tue, 09 Jun 2020 20:39:40 GMT  
		Size: 55.4 MB (55409567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:7faf045b6160c541529a0229a1afe28a3693560048d5ff1848b5321fafb22953
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.9 MB (392876687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec4a12b28dd2208a12434c73008c09b918476b12a45f7b84620925a7e910f44c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 22 Jul 2020 00:43:42 GMT
ADD file:9c5c9df9952cb51291333837bdb462bbdf9f157e91e616f1e3fb8d2fcb1a1983 in / 
# Wed, 22 Jul 2020 00:43:45 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 19:25:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 19:25:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 22 Jul 2020 19:26:02 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 22 Jul 2020 19:26:10 GMT
ENV LANG=C.UTF-8
# Wed, 22 Jul 2020 19:26:14 GMT
ENV LC_ALL=C.UTF-8
# Wed, 22 Jul 2020 19:26:16 GMT
ENV ROS_DISTRO=melodic
# Wed, 22 Jul 2020 19:30:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 19:30:08 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 22 Jul 2020 19:30:18 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 22 Jul 2020 19:30:23 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 19:31:34 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 19:31:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 22 Jul 2020 19:33:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ad4de4f68e9c2c0f5e5e62d379d936bb88ce467505ed002fb1e10c434fefe90c`  
		Last Modified: Wed, 22 Jul 2020 00:49:52 GMT  
		Size: 43.2 MB (43169407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585176f5de99b8e33359e78fe9cd34f20da6cf5724e665a8f2298c4e08a2c01f`  
		Last Modified: Wed, 22 Jul 2020 19:58:33 GMT  
		Size: 6.4 MB (6438780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03065d637722b646c143464a227682878b2e718150a24a8330bf249ea91391ef`  
		Last Modified: Wed, 22 Jul 2020 19:58:29 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:682b45741119383dec6695aefd378294f6b562056f0339f1f1955db84f2001e0`  
		Last Modified: Wed, 22 Jul 2020 19:58:29 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a464bacf6f2264fb00064f902ee0a88ab0809f727acda3fa174eee7c97595e`  
		Last Modified: Wed, 22 Jul 2020 19:59:57 GMT  
		Size: 225.0 MB (224953934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2acfe8e8d7f95c79bbcb21d3a9f931ee58d52bee040afac16b87be02b940003`  
		Last Modified: Wed, 22 Jul 2020 19:58:31 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:243df2136f331d3be62549924b6e4bb6b48cef2919e840054c5b8a810cb0ba1e`  
		Last Modified: Wed, 22 Jul 2020 20:00:24 GMT  
		Size: 64.8 MB (64836222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79c43b3fca6d5121261cd09c44c321c34a02208fae74092b1690d18ef9694cc`  
		Last Modified: Wed, 22 Jul 2020 20:00:04 GMT  
		Size: 253.8 KB (253849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a76dc9ae5004d0aff32a490571832256bb63fcb072c618b7a7a3a1fc72025b8`  
		Last Modified: Wed, 22 Jul 2020 20:00:23 GMT  
		Size: 53.2 MB (53222677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
