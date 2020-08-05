## `ros:melodic-ros-base-stretch`

```console
$ docker pull ros@sha256:abb5d832c7e9598d2801da991f11bb9affbad3d8d41851d8665aa82e97f281c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-stretch` - linux; amd64

```console
$ docker pull ros@sha256:18ee16ffb4b877dc6e0c8acbf9c8326d9abed50ed77ae740e6990571e8a8e526
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **447.6 MB (447583700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17c3d0cd7ec176a91b7b01021f95fb8ca963134ccf0bac81656ee73c6b77140b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 15:45:32 GMT
ADD file:a28d8a949b7577768d87fcbac346797fc5f7bad0539625339edcd09a32d6bf77 in / 
# Tue, 04 Aug 2020 15:45:33 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 06:46:56 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 06:46:59 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 05 Aug 2020 06:47:00 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 05 Aug 2020 06:47:00 GMT
ENV LANG=C.UTF-8
# Wed, 05 Aug 2020 06:47:00 GMT
ENV LC_ALL=C.UTF-8
# Wed, 05 Aug 2020 06:47:01 GMT
ENV ROS_DISTRO=melodic
# Wed, 05 Aug 2020 06:48:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 06:48:26 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 05 Aug 2020 06:48:26 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 05 Aug 2020 06:48:26 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 06:48:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 06:49:05 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 05 Aug 2020 06:49:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:419e7ae5bb1e4875c367f3249b7bb7f8f39dd27dfceb4ee9d6a92191ed1c452f`  
		Last Modified: Tue, 04 Aug 2020 15:52:05 GMT  
		Size: 45.4 MB (45366706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae70a4ac92afa745eca40bc9c10b2b1a4178e76b079107c67dfc365e8b9cc37`  
		Last Modified: Wed, 05 Aug 2020 07:02:16 GMT  
		Size: 6.9 MB (6866461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd09b8777edb3312770ea102d89becdbaa8ce1405c8ca848c91be9864b21698c`  
		Last Modified: Wed, 05 Aug 2020 07:02:14 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f33914001586acf8a14dbdf92edba1c9ff4ff86098a74b288072d18c613283`  
		Last Modified: Wed, 05 Aug 2020 07:02:14 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be21922ef3a7cbaf6d454d3ca6fba32f59401db9c03952f4dd656287dc998acf`  
		Last Modified: Wed, 05 Aug 2020 07:03:09 GMT  
		Size: 269.9 MB (269884481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16bcb18292043bc82bd5f157326157ad4a247d9363205ce280e385bcd78211e`  
		Last Modified: Wed, 05 Aug 2020 07:02:14 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9dc886291df81c830f0d28e977360c32e55df94297731a56c479fcc9f5d70e`  
		Last Modified: Wed, 05 Aug 2020 07:03:30 GMT  
		Size: 70.2 MB (70152019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd4eea30525fcc35113c2c676a3141c698b401cd91adf7dd8a9791ba9865463b`  
		Last Modified: Wed, 05 Aug 2020 07:03:17 GMT  
		Size: 254.9 KB (254861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2067ba19771c54d437f34613c52ea1085c621cec0fdf654ef292bc3b02f3d4`  
		Last Modified: Wed, 05 Aug 2020 07:03:29 GMT  
		Size: 55.1 MB (55057354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d63713af1ebb69b3e004c4993232a49c5b998f98ff7517eae3fdc850e29366ff
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.9 MB (392891726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0eedea8580a3526b54f9107e9b8405224733ef99709c8389fff10c4c9de4b9fc`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:59:38 GMT
ADD file:0a7a65de4c9dc6ea7f7ac97362a47b82a02a45ecab668ddc84cfd011dad26d33 in / 
# Tue, 04 Aug 2020 06:59:41 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 10:02:17 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 10:02:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 04 Aug 2020 10:02:24 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 04 Aug 2020 10:02:25 GMT
ENV LANG=C.UTF-8
# Tue, 04 Aug 2020 10:02:25 GMT
ENV LC_ALL=C.UTF-8
# Tue, 04 Aug 2020 10:02:26 GMT
ENV ROS_DISTRO=melodic
# Tue, 04 Aug 2020 10:05:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 10:05:49 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 04 Aug 2020 10:05:51 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 04 Aug 2020 10:05:56 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 10:06:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 10:07:24 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 04 Aug 2020 10:08:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:708f9b01fc1a5dff70f7d40443ac7dd0ee1d0ae93202b6f305f4e3627cea7d22`  
		Last Modified: Tue, 04 Aug 2020 07:06:12 GMT  
		Size: 43.2 MB (43171643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac412b2554318f4b6050db40ac7104b507a6e40edba068b5a1c3e30ffdf3c35e`  
		Last Modified: Tue, 04 Aug 2020 10:31:28 GMT  
		Size: 6.4 MB (6438845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01136f9bde07ae51236af3dbff422307927028bbc5414c25554993f0595bac8a`  
		Last Modified: Tue, 04 Aug 2020 10:31:26 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a1883d43a0d6aeea6bba737aa6c11a01844b88be21462e4055ccb98e91d892`  
		Last Modified: Tue, 04 Aug 2020 10:31:26 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90009b0420756860fcd9aa0ce9221d6c3972877e576855a480e34a4e4281651`  
		Last Modified: Tue, 04 Aug 2020 10:32:37 GMT  
		Size: 225.0 MB (224953525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736029edcfd0de1adc7218032511d84d44a5cf7909c2de0c35f3e311ee13292d`  
		Last Modified: Tue, 04 Aug 2020 10:31:26 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f52684428f2f1c5ddb65bb4ac4804d92e6f187ad94a5500e31d3f9522ca120c`  
		Last Modified: Tue, 04 Aug 2020 10:33:00 GMT  
		Size: 64.8 MB (64840268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df4438146edf4f0172672fb2eed6b4759c6dd5807cba1560f036b0476054e68`  
		Last Modified: Tue, 04 Aug 2020 10:32:43 GMT  
		Size: 254.9 KB (254908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd47fd5638bcf1fa58b899ba6e5cc0ae8479595dff5c3c3c65b35bab46c1c25`  
		Last Modified: Tue, 04 Aug 2020 10:33:15 GMT  
		Size: 53.2 MB (53230719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
