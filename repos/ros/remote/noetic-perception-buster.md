## `ros:noetic-perception-buster`

```console
$ docker pull ros@sha256:b917b8afa207e0932de817b5ed403cea0daa3a2edc3b494a08a941cf70680843
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-perception-buster` - linux; amd64

```console
$ docker pull ros@sha256:118ea7c7ae6390acd2aded6d156de90bdd4ee8a4b1c6761db9477a6cc082a6cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **951.2 MB (951209677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20541cbb2cb1454e3836c081c246aaf6c41c38f9e0f5e43524b27652476bfa79`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:41 GMT
ADD file:c865da7afcf35b5a9538e63633f7e99ae4c40933cb8a0235e9704713042fba66 in / 
# Wed, 21 Dec 2022 01:20:42 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 11:00:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:00:07 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 21 Dec 2022 11:00:09 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 21 Dec 2022 11:00:09 GMT
ENV LANG=C.UTF-8
# Wed, 21 Dec 2022 11:00:09 GMT
ENV LC_ALL=C.UTF-8
# Wed, 21 Dec 2022 11:00:09 GMT
ENV ROS_DISTRO=noetic
# Wed, 21 Dec 2022 11:01:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:01:37 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 21 Dec 2022 11:01:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 21 Dec 2022 11:01:37 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 11:02:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:02:18 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 21 Dec 2022 11:03:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:07:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c7c50787e2da71205402343dd1233b3ca6ebe70c7e790f6ba7d856b81b893200`  
		Last Modified: Wed, 21 Dec 2022 01:24:55 GMT  
		Size: 50.4 MB (50448893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b052e3063dd5e1f5dd43ac9327c08a1f0ba5c05673755f0ddbc54eb8a47b68ed`  
		Last Modified: Wed, 21 Dec 2022 11:08:36 GMT  
		Size: 10.9 MB (10896939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83902353ad66fb52936b96293c207b00d5b37b587f35948ca0a2e679a1f0a0e`  
		Last Modified: Wed, 21 Dec 2022 11:08:34 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cadf3ead30322d6c27a63204270292209d103c528b40928749587f9d7e136a`  
		Last Modified: Wed, 21 Dec 2022 11:08:34 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53c16a3a9b3a8fe00067d85297c8380ad068e3b1f484b284f35f9d54feaa04d`  
		Last Modified: Wed, 21 Dec 2022 11:09:08 GMT  
		Size: 239.2 MB (239205442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9168ac3a9e93b34a9b55bbd10385b07a62b2e6d6cc2c2ea2fde52bae7aeb96`  
		Last Modified: Wed, 21 Dec 2022 11:08:34 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574b7ce55ba7fdaaeec166ec647f6340cc91a1a2e51d56611321212e582fc441`  
		Last Modified: Wed, 21 Dec 2022 11:09:30 GMT  
		Size: 86.6 MB (86603015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e570d3835677549b55dae60d3bde8885640704299063b3c01e2f7fcb51c7ba`  
		Last Modified: Wed, 21 Dec 2022 11:09:17 GMT  
		Size: 334.8 KB (334763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42887f47d573625da7116cd5dd3aac01fdd922e84fb04cb757dc6f62ae7637fa`  
		Last Modified: Wed, 21 Dec 2022 11:09:28 GMT  
		Size: 76.0 MB (75978042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfeebe1fcaed8ad561cfb4d7dd2eac4b207065e33f753942df31c82b82018cf5`  
		Last Modified: Wed, 21 Dec 2022 11:10:58 GMT  
		Size: 487.7 MB (487740170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:68148b43392cedc2ac5baeff8fbebfb5840ca68d43fa388b9170dbe8ae03b766
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **868.0 MB (868008808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa505f56ea448629dc64c0356a62615858454c77bc271486eda5250e49375fbd`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:54 GMT
ADD file:2129940567ffc1f6fc724b59b8ab1f337db54cd9164e50494822bcedd46d85c7 in / 
# Wed, 21 Dec 2022 01:39:55 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 12:12:30 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 12:12:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 21 Dec 2022 12:12:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 21 Dec 2022 12:12:32 GMT
ENV LANG=C.UTF-8
# Wed, 21 Dec 2022 12:12:32 GMT
ENV LC_ALL=C.UTF-8
# Wed, 21 Dec 2022 12:12:32 GMT
ENV ROS_DISTRO=noetic
# Wed, 21 Dec 2022 12:13:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 12:13:49 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 21 Dec 2022 12:13:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 21 Dec 2022 12:13:49 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 12:14:19 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 12:14:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 21 Dec 2022 12:15:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 12:19:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ebd367421c805cd84d245a61615aeaa29bb9c2fdbdb111a373ee13b9934d9cf9`  
		Last Modified: Wed, 21 Dec 2022 01:43:31 GMT  
		Size: 49.2 MB (49233817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08619936cad6d315f51012474fa22f2fd8f1b475904aeeff8ab1ac9c94fb0770`  
		Last Modified: Wed, 21 Dec 2022 12:20:30 GMT  
		Size: 10.9 MB (10902542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49515cbca6d7dbd9df1f61795afce1f6540a7a7311f1e810e4e6119c9fe2b775`  
		Last Modified: Wed, 21 Dec 2022 12:20:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b1d3f149f7c168a510f4e797a86641439ab36f1672b64c32293d7f8c8501bc`  
		Last Modified: Wed, 21 Dec 2022 12:20:29 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843956780ad36f94b7e0b598faa8c34f95b66ed491d15dc1b1d415e442f55810`  
		Last Modified: Wed, 21 Dec 2022 12:20:52 GMT  
		Size: 184.4 MB (184388328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689420f0e90e19012bdbc76769c6d25d3029bb1789f3f4e11b26ddfc71c98cb5`  
		Last Modified: Wed, 21 Dec 2022 12:20:29 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cafe663c78ec8ec83680ea83b1eb1d875557336eaa0250b7da09cf2a31a73a9`  
		Last Modified: Wed, 21 Dec 2022 12:21:07 GMT  
		Size: 84.4 MB (84392573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed64ee0e529545d23cbf4774ca33327a650a6c43ac3538b89be5f1c573c6d3f`  
		Last Modified: Wed, 21 Dec 2022 12:20:58 GMT  
		Size: 334.8 KB (334765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bb1fb353f747aa2cdd4952aa366c48c03fd0a22dc2a88790e59ba8edd5c98d`  
		Last Modified: Wed, 21 Dec 2022 12:21:06 GMT  
		Size: 74.1 MB (74089601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c304188c356ac7ab29c9db8f7e634caeaf378e55c425f6044983ee201bdac1`  
		Last Modified: Wed, 21 Dec 2022 12:22:11 GMT  
		Size: 464.7 MB (464664770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
