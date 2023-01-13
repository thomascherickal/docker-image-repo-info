## `ros:galactic-ros1-bridge`

```console
$ docker pull ros@sha256:7dc3a60c1a2459a2631262a395685a05a8c6bab5731be5a0bdb71ec25ad940d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:af0a024e8159bf4048658bb1e1e5ed969f632d36685421aa4c2d8cdf77ae6793
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.2 MB (330218444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c07229329d7da164d8cef51585a7b5f104c1130d9feaf041b86b1dd3f4a3ad2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:05:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:56:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 23:20:30 GMT
RUN echo "deb http://snapshots.ros.org/galactic/final/ubuntu focal main" > /etc/apt/sources.list.d/ros2-snapshots.list
# Thu, 12 Jan 2023 23:20:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Thu, 12 Jan 2023 23:20:31 GMT
ENV LANG=C.UTF-8
# Thu, 12 Jan 2023 23:20:31 GMT
ENV LC_ALL=C.UTF-8
# Thu, 12 Jan 2023 23:20:31 GMT
ENV ROS_DISTRO=galactic
# Thu, 12 Jan 2023 23:22:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 23:22:28 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 12 Jan 2023 23:22:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 12 Jan 2023 23:22:28 GMT
CMD ["bash"]
# Thu, 12 Jan 2023 23:23:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 23:23:26 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 12 Jan 2023 23:23:31 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 12 Jan 2023 23:24:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 23:24:16 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 12 Jan 2023 23:24:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 12 Jan 2023 23:24:17 GMT
ENV ROS1_DISTRO=noetic
# Thu, 12 Jan 2023 23:24:18 GMT
ENV ROS2_DISTRO=galactic
# Thu, 12 Jan 2023 23:25:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.15-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 23:25:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.4-1*     ros-galactic-demo-nodes-py=0.14.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 23:25:49 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caabce4ffd25edf36993bf0280efcd423502afe7b8c7b2da5782388b72f81a89`  
		Last Modified: Fri, 09 Dec 2022 02:17:31 GMT  
		Size: 1.2 MB (1154736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c569c2442d05771daee8e23d1b056915b3dc9dd15887bfc5723720f10c7a6`  
		Last Modified: Fri, 09 Dec 2022 05:34:20 GMT  
		Size: 5.6 MB (5551517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18533ac4b95004ac48f1ae8e3cd0f52b628285c5c99212a9ccaf8309191fc2b4`  
		Last Modified: Thu, 12 Jan 2023 23:27:05 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f73489d6d95d231ecd0b99ba2939cfc514babae220fee00a8f1d80ef672c52`  
		Last Modified: Thu, 12 Jan 2023 23:27:05 GMT  
		Size: 2.4 KB (2400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48804199734bb0d8cd7c3acbc6d13b6081ffb975eed61ed44ed2e224edb57f19`  
		Last Modified: Thu, 12 Jan 2023 23:27:22 GMT  
		Size: 104.0 MB (104015431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790366988bec99064529cc4474b7f53f27ffe8c92d9cef9567b6a4740afebd34`  
		Last Modified: Thu, 12 Jan 2023 23:27:05 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550e38a77050a74c88ab5baebc67883038a5a2c36df6a4a845a90b77294be72d`  
		Last Modified: Thu, 12 Jan 2023 23:27:41 GMT  
		Size: 73.3 MB (73281982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf6b2ec67f9ba7084cbd94736b2ded712b84c693e3af84740dec6fe6b43b57c`  
		Last Modified: Thu, 12 Jan 2023 23:27:30 GMT  
		Size: 286.8 KB (286806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce271229f391ba190d41191da9052d179fec64b188703d43494765d47de6fc53`  
		Last Modified: Thu, 12 Jan 2023 23:27:30 GMT  
		Size: 2.4 KB (2422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b155ebe6e75431ab14999376865e08e21b5994a610e5d1b85632cc2711c2a803`  
		Last Modified: Thu, 12 Jan 2023 23:27:33 GMT  
		Size: 22.1 MB (22140177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d820349bdaa6c4e69089544d27172850eab2c29fbffb169afe150da68c1046bd`  
		Last Modified: Thu, 12 Jan 2023 23:27:52 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd6e692d1ce3fba0933e030376c12cd7513bcea76c384463d495189fe9886d5`  
		Last Modified: Thu, 12 Jan 2023 23:27:53 GMT  
		Size: 4.2 KB (4170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161fd6589b6c8dc0836d0f0b1a9b7179095c531857564ffb8b9651c6bca65811`  
		Last Modified: Thu, 12 Jan 2023 23:28:07 GMT  
		Size: 78.7 MB (78708763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293e6fb441cd403380c28258e88fd86b0784fdb3aa39487dac55052b8a061957`  
		Last Modified: Thu, 12 Jan 2023 23:27:56 GMT  
		Size: 16.5 MB (16492252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2289bd462e3195ff31e1ee37befc1600c62f76587bc4001f0d0848da2bd8460`  
		Last Modified: Thu, 12 Jan 2023 23:27:52 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ddaf44c4a2c4abac1ec3dafb34d0354f3a9dbdcd765da6f27e1164d933e4912f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.4 MB (318398929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d592a410d0eaf468005847704dd7847b5e0bbff313d9b723d50668d6fe5119d7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:43:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 22:47:38 GMT
RUN echo "deb http://snapshots.ros.org/galactic/final/ubuntu focal main" > /etc/apt/sources.list.d/ros2-snapshots.list
# Thu, 12 Jan 2023 22:47:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Thu, 12 Jan 2023 22:47:40 GMT
ENV LANG=C.UTF-8
# Thu, 12 Jan 2023 22:47:40 GMT
ENV LC_ALL=C.UTF-8
# Thu, 12 Jan 2023 22:47:40 GMT
ENV ROS_DISTRO=galactic
# Thu, 12 Jan 2023 22:49:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 22:49:46 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 12 Jan 2023 22:49:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 12 Jan 2023 22:49:47 GMT
CMD ["bash"]
# Thu, 12 Jan 2023 22:50:47 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 22:50:51 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 12 Jan 2023 22:50:56 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 12 Jan 2023 22:51:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 22:51:54 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 12 Jan 2023 22:51:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 12 Jan 2023 22:51:55 GMT
ENV ROS1_DISTRO=noetic
# Thu, 12 Jan 2023 22:51:55 GMT
ENV ROS2_DISTRO=galactic
# Thu, 12 Jan 2023 22:53:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.15-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 22:53:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.4-1*     ros-galactic-demo-nodes-py=0.14.4-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 22:53:28 GMT
COPY file:196e0ab4e3b32a1af101eff4dfa0110eb39feb70f4f9f2df3de2e22162513085 in / 
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757fb2fe2f280d64cc7c0734dadd7f72dfcd73d70d14dce449f6ec2e6834b66f`  
		Last Modified: Fri, 09 Dec 2022 03:22:59 GMT  
		Size: 1.2 MB (1154754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34108aa9b6e179025d554465ed41e434532d83865bdc22a0b4ea074748d69d1e`  
		Last Modified: Fri, 09 Dec 2022 03:22:58 GMT  
		Size: 5.5 MB (5531057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a7cf1cc80ad37b196dcfab47ce981ee43aee45d8adce1fe8783373db322f4f7`  
		Last Modified: Thu, 12 Jan 2023 22:54:45 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffc6fa3e2aa1aa444e384d7b35e8fb1c4b52228f2e538fd942fd1d04d68ff9e`  
		Last Modified: Thu, 12 Jan 2023 22:54:45 GMT  
		Size: 2.4 KB (2399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84dd4a45fa6f8dfc5845bfa1fba3da4f4b8ec7b350322177e531ef8e8123d5e`  
		Last Modified: Thu, 12 Jan 2023 22:54:58 GMT  
		Size: 100.4 MB (100436911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9512977316ac0bcb88c6cbcd892f02cea92cb2085b9bcebdfa1ee802d64fd09c`  
		Last Modified: Thu, 12 Jan 2023 22:54:45 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9113d4a0236b030f0d0cc85538774efbfe92146011fcd51e23014b1f46dbd8d2`  
		Last Modified: Thu, 12 Jan 2023 22:55:15 GMT  
		Size: 67.6 MB (67618595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ba95396220efca37ee104e9d5a43ac70ab5c04f6fc77781d7cd7534018ce19`  
		Last Modified: Thu, 12 Jan 2023 22:55:07 GMT  
		Size: 286.8 KB (286806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2724439fe0b2182f32487961c19ee7133913463ff712cf0e8d3814f9109e338`  
		Last Modified: Thu, 12 Jan 2023 22:55:07 GMT  
		Size: 2.4 KB (2421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ef5a332708ffdd8dd39d8e05cc708046ca3d323b3e8565f410008a11099c12`  
		Last Modified: Thu, 12 Jan 2023 22:55:10 GMT  
		Size: 21.5 MB (21481415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30f7464da9a42f5445ec5fc7b38cde64ef3c0bbc844687ec0c4c3ef469accb6`  
		Last Modified: Thu, 12 Jan 2023 22:55:26 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797240e96890e87cf998c5ef1de371015aae64d6814837d6b3624d59a2be17c0`  
		Last Modified: Thu, 12 Jan 2023 22:55:26 GMT  
		Size: 4.2 KB (4169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84f8f553c8579dd3a2bf0a624fb19a72418b0cceb887d12fe6dd68125c513cd`  
		Last Modified: Thu, 12 Jan 2023 22:55:37 GMT  
		Size: 78.7 MB (78674135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc31888de3b1066a563a79439df36d6424141e190f88d6c877b0b3798a51550`  
		Last Modified: Thu, 12 Jan 2023 22:55:28 GMT  
		Size: 16.0 MB (16012197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79350f37505230af98f2ee675eea66d70b6f1add843128ebb090df8842d37a1c`  
		Last Modified: Thu, 12 Jan 2023 22:55:26 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
