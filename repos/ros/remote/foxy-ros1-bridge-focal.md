## `ros:foxy-ros1-bridge-focal`

```console
$ docker pull ros@sha256:a2ae48ba0e805548aba576d7da33e5a7eb558af3fe828b1fb1c27732d6545dfd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy-ros1-bridge-focal` - linux; amd64

```console
$ docker pull ros@sha256:ad49d5486d4f18c27bbd5a43e9c82eee8c870f15a629315884ee95be61542b62
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.0 MB (349019600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af0fba0f6333ea96c55c3744fd2c72b3688f12d19912764dc502ddb242acde1c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 26 Jan 2023 13:19:55 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:19:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:19:57 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Thu, 26 Jan 2023 13:19:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 19:29:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:30:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:43:09 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Tue, 31 Jan 2023 19:43:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:43:10 GMT
ENV LANG=C.UTF-8
# Tue, 31 Jan 2023 19:43:10 GMT
ENV LC_ALL=C.UTF-8
# Tue, 31 Jan 2023 19:43:11 GMT
ENV ROS_DISTRO=foxy
# Tue, 31 Jan 2023 19:44:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:44:11 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Tue, 31 Jan 2023 19:44:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 31 Jan 2023 19:44:11 GMT
CMD ["bash"]
# Tue, 31 Jan 2023 19:44:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:44:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 31 Jan 2023 19:44:51 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Tue, 31 Jan 2023 19:45:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:45:16 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 31 Jan 2023 19:45:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 31 Jan 2023 19:45:18 GMT
ENV ROS1_DISTRO=noetic
# Tue, 31 Jan 2023 19:45:18 GMT
ENV ROS2_DISTRO=foxy
# Tue, 31 Jan 2023 19:45:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.15-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:45:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 19:45:57 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c07949706a41bd26517c40195af4c4877c4a94497526c106a6293763dc1765b`  
		Last Modified: Tue, 31 Jan 2023 20:08:43 GMT  
		Size: 1.2 MB (1154542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2670e9e05f7f793dd7dbe48fba615b13142ad5665135c312378240da79579b`  
		Last Modified: Tue, 31 Jan 2023 20:08:41 GMT  
		Size: 5.6 MB (5553673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf152e9a4db74f9930ac09483751214af9a1f226e0fb2a2d70369627cb6ddf8`  
		Last Modified: Tue, 31 Jan 2023 20:11:16 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59cc39066911af026fbfacd58275ced54dc5087430530321ace88cd70eb17d4`  
		Last Modified: Tue, 31 Jan 2023 20:11:16 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53c5af39e4f0d50dd2e34266f9a2a903ddf6ff3fb23360d78ab392d946b5115`  
		Last Modified: Tue, 31 Jan 2023 20:11:36 GMT  
		Size: 120.4 MB (120354163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f77ccef24b2168378b7993b994be148d7ccc81dcc0dd6af02b3498a508ad4a`  
		Last Modified: Tue, 31 Jan 2023 20:11:16 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c587bd24e6d3bd17af2906318935c23cec69372158c04d4c0e2276c45f79a1f8`  
		Last Modified: Tue, 31 Jan 2023 20:11:55 GMT  
		Size: 73.3 MB (73334209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9589f9c9bae39b4cbb571d2095fa9e20972d7bedf34f56c71cb377b234aa7207`  
		Last Modified: Tue, 31 Jan 2023 20:11:45 GMT  
		Size: 277.8 KB (277778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a06edf09eaea7b0d1b06ccd74d1c8af33e67656d5a32341b70f778dfa2fc7e17`  
		Last Modified: Tue, 31 Jan 2023 20:11:45 GMT  
		Size: 2.4 KB (2432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20917058504694a3791959dd4dc87db6cd42cf6c632019971eea5c6474b355c2`  
		Last Modified: Tue, 31 Jan 2023 20:11:48 GMT  
		Size: 21.7 MB (21662318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac032e991d1161d607d3070d68fdb31d6002bc5fbc2c7c2d8faca77f92376c56`  
		Last Modified: Tue, 31 Jan 2023 20:12:07 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab4f85c71b205725d550cb61dab91e859f5c7d09b9360d91d5cf51267f6facd`  
		Last Modified: Tue, 31 Jan 2023 20:12:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1fd5b2feb27aedbe99d898da57948097f733170938a3b3e78d19cf5c993086`  
		Last Modified: Tue, 31 Jan 2023 20:12:21 GMT  
		Size: 76.4 MB (76425495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b22a19e3db8effb381b6add35af1ed189384797e8fbf54248a4ecc847e06f5`  
		Last Modified: Tue, 31 Jan 2023 20:12:11 GMT  
		Size: 21.7 MB (21674062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1888223ca45436cd56eeea009914eb481039a545fa94fa0765ab08841a5310d4`  
		Last Modified: Tue, 31 Jan 2023 20:12:07 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy-ros1-bridge-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:d613d38696ab3c45d22678d6ce5adb76673fad8cf53a536da222be4b80d05a56
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.6 MB (317605237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c6a1bd93bbc2c863ca9d150026991c1bafe61190cf7b6500d84c66216dde544`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:14:25 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:14:30 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:27:19 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 01 Feb 2023 19:27:20 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 19:27:20 GMT
ENV LANG=C.UTF-8
# Wed, 01 Feb 2023 19:27:20 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Feb 2023 19:27:20 GMT
ENV ROS_DISTRO=foxy
# Wed, 01 Feb 2023 19:28:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:28:13 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 01 Feb 2023 19:28:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Feb 2023 19:28:13 GMT
CMD ["bash"]
# Wed, 01 Feb 2023 19:28:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:28:37 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 01 Feb 2023 19:28:42 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 01 Feb 2023 19:28:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:29:04 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 01 Feb 2023 19:29:05 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 19:29:05 GMT
ENV ROS1_DISTRO=noetic
# Wed, 01 Feb 2023 19:29:06 GMT
ENV ROS2_DISTRO=foxy
# Wed, 01 Feb 2023 19:29:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.15-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:29:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros1-bridge=0.9.6-1*     ros-foxy-demo-nodes-cpp=0.9.4-1*     ros-foxy-demo-nodes-py=0.9.4-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:29:39 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c8f9dc33001d56b88f13d7fd593e7bcf0326e85fbc90187faeb3a478742e54`  
		Last Modified: Wed, 01 Feb 2023 19:30:51 GMT  
		Size: 1.2 MB (1154586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3873cd7c37c05b51f3da3a7ac1f74b5b79d8fb0edf778ce3559a6b0e5116669`  
		Last Modified: Wed, 01 Feb 2023 19:30:50 GMT  
		Size: 5.5 MB (5531974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35822ce940b9704c5e562c8885cd4237afaf6e84b90f7c48668268d02841317a`  
		Last Modified: Wed, 01 Feb 2023 19:32:52 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a96b499a409fee7868ba33436e1e349aa7105196b48c5d28176255c349eee2`  
		Last Modified: Wed, 01 Feb 2023 19:32:53 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e27291a08fcede5386841e1e5b0584c094cd548e062f278776bbbae3a45c6a80`  
		Last Modified: Wed, 01 Feb 2023 19:33:06 GMT  
		Size: 104.6 MB (104557994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb93a26a5fab9482f321f676d17a8702539d7b32e7194ddc4879739f1425ed9`  
		Last Modified: Wed, 01 Feb 2023 19:32:52 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7adda8a81e2bf6c30215882e975243f6a170a540c87e8c7e3b1332fa416972c`  
		Last Modified: Wed, 01 Feb 2023 19:33:22 GMT  
		Size: 67.7 MB (67681881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec47ba32a1ca970ab95560eed5fda1d4f9f03b051a6e7339297c5d0ff2508bb`  
		Last Modified: Wed, 01 Feb 2023 19:33:15 GMT  
		Size: 277.8 KB (277778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1ce524890c3bf979cb77c26228586bc1657bdd90214e8cceb0cadbf8808fad`  
		Last Modified: Wed, 01 Feb 2023 19:33:14 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bbba78bc114f5f6afc240ad05c8b56ce878ebf866200090d533ec6620ac128`  
		Last Modified: Wed, 01 Feb 2023 19:33:17 GMT  
		Size: 20.4 MB (20384862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb743e68e44180e01c844a18c62383859bd90cfecbf975e6d3514143b1b5b16`  
		Last Modified: Wed, 01 Feb 2023 19:33:33 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb68ff40f9ab643b646bdd28ac51b25ae5d4b5172e71a895ce932cb09f11f936`  
		Last Modified: Wed, 01 Feb 2023 19:33:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc63d3f2a453d56ffc84be29895fc86fe9147f526e418b9a54c7e5d2102949a`  
		Last Modified: Wed, 01 Feb 2023 19:33:45 GMT  
		Size: 76.5 MB (76491984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e733adf20852512138fea893a09497b474e5e2eb66c426b7e20d8a6fabc148`  
		Last Modified: Wed, 01 Feb 2023 19:33:36 GMT  
		Size: 14.3 MB (14324939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131efeacb312fb02072a1ab567a7e9aba2cfb394a98d8d6e7dfdf5f76455d9dc`  
		Last Modified: Wed, 01 Feb 2023 19:33:33 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
