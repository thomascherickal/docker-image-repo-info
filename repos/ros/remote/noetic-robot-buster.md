## `ros:noetic-robot-buster`

```console
$ docker pull ros@sha256:b3e21be29ba770550632b2660e89eb534689f5719b99e464036351e15e68af26
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-robot-buster` - linux; amd64

```console
$ docker pull ros@sha256:5a7f86c927079a5680dc6894240b166341ccd35b5e783083e83c065061eccc01
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.6 MB (484624407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16f97007696a1b2771f425f817c07e7a6f54a8200cde3fb9f660a51027e2ffdc`
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
# Wed, 21 Dec 2022 11:03:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:97947107aba0f0467ae57bae9eb05f15f95582dfc840921ade777ad411375019`  
		Last Modified: Wed, 21 Dec 2022 11:09:38 GMT  
		Size: 21.2 MB (21154900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:699858e1b85182436683b2629c4c430a40579f502d65c6b6df0cd78c5f8b14a8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **424.2 MB (424161781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:571dd4b77e50e35193ffe4f09ad47ef91b10f162a0ba98358a7ece34a35cbbb9`
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
# Wed, 21 Dec 2022 12:15:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:c3f2ac528ed2ea48347b30f1fbcf4319d1c92f7e84aa5ae6c74bb78ed0bca7a0`  
		Last Modified: Wed, 21 Dec 2022 12:21:15 GMT  
		Size: 20.8 MB (20817743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
