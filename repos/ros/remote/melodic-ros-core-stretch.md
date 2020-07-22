## `ros:melodic-ros-core-stretch`

```console
$ docker pull ros@sha256:b80b9d0af01d116c0867c4a5824f30b94c6586cee92793e465b9d049ac8b2803
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-stretch` - linux; amd64

```console
$ docker pull ros@sha256:d16d411c2de4bdb9dbd792e146be49cbc6801321829ea16a825215df35eb5be8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.1 MB (322059503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3816f11bdde39731fba61a16ee620c21d47f9d0e706a50275d2e8c2d2283753`
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

### `ros:melodic-ros-core-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:afd5a1e3d5bf6f2d5a432a9e143cbb2c623334caf55a4b97fee2c96a871c32e2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.6 MB (274563939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb4da1e59e04ea0ac3264c2bdb24c5e4959e1075b9a0e49ea3823185364dfd69`
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
