## `ros:melodic-robot-stretch`

```console
$ docker pull ros@sha256:7b7e31e6d376d30616eeef5bcc919c98ef705d5f7af4785c382ac27e5a256654
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-robot-stretch` - linux; amd64

```console
$ docker pull ros@sha256:41085b86087bffadaf3aa25a182d21ff18d23544f14d68b2da6e29e7a944ede6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.0 MB (463003832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fddd4cd5232e7c58870093da429b3ecf27bdc5980ba26cc003ef9261e05440b2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:33:25 GMT
ADD file:13031623172f5c5857e27de93553adedf17d955fa370882f850bb6ed6fb8cee7 in / 
# Fri, 15 May 2020 06:33:25 GMT
CMD ["bash"]
# Wed, 27 May 2020 00:40:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 27 May 2020 00:40:24 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 27 May 2020 00:40:25 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 27 May 2020 00:40:25 GMT
ENV LANG=C.UTF-8
# Wed, 27 May 2020 00:40:25 GMT
ENV LC_ALL=C.UTF-8
# Wed, 27 May 2020 00:40:25 GMT
ENV ROS_DISTRO=melodic
# Wed, 27 May 2020 00:41:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 May 2020 00:41:55 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 27 May 2020 00:41:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 27 May 2020 00:41:56 GMT
CMD ["bash"]
# Wed, 27 May 2020 00:42:31 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 27 May 2020 00:42:37 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 27 May 2020 00:43:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 27 May 2020 00:43:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1c6172af85ee14a8db5a3a51d406b768dfa94d196c06d0d06d591507cf8199f0`  
		Last Modified: Fri, 15 May 2020 06:40:31 GMT  
		Size: 45.4 MB (45375207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b28b20c8c413ed647ed74f3f10133be8da4590c9925bf94a9d2319ffb2f7a8f`  
		Last Modified: Wed, 27 May 2020 00:56:31 GMT  
		Size: 6.9 MB (6865154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2a66cab0412b434c4a2500c5cec7decca877232cc612f58d7e4b73609be25b`  
		Last Modified: Wed, 27 May 2020 00:56:29 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeebda54a351b9b0cfeed08f111e7c8499bd2df81854da04d1e381ac5a3d7802`  
		Last Modified: Wed, 27 May 2020 00:56:30 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef33ca1dc9083382ef51b03efe176f7b62118f29b79b53ec1bcd8826e1539b82`  
		Last Modified: Wed, 27 May 2020 00:57:23 GMT  
		Size: 269.9 MB (269864464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cfe8e8aa3afa6faf61324475cebe6fdc50502c69491f443342ba48f33127c1e`  
		Last Modified: Wed, 27 May 2020 00:56:30 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7f72e40487afc172f24e1502e68b3997a0705af028d54062439ae655373c8e`  
		Last Modified: Wed, 27 May 2020 00:57:41 GMT  
		Size: 70.2 MB (70150269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aff17de8219cffc22ee1df7ccc29b1ac3d2f19bdd7a404452d58dde21db6490`  
		Last Modified: Wed, 27 May 2020 00:57:27 GMT  
		Size: 248.1 KB (248106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f117343e149e4c9132c0d85084fc0ca2ee5d8e4ccf367bb179b8891ba0c2a97e`  
		Last Modified: Wed, 27 May 2020 00:57:40 GMT  
		Size: 55.4 MB (55407140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321c4c2ec3be7ad90593a332d84d9b6f1378e43a3ee810c7dd2020fd31f0bb5a`  
		Last Modified: Wed, 27 May 2020 00:57:47 GMT  
		Size: 15.1 MB (15091680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f2c96cf75b7d5b4724b273239ef66a8b36c9df49a7da4021db4a5a9c44c8f8be
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **464.7 MB (464718138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06f676e65839210a7ee1222e2253d6fb5e3b9ca5b6da1eb9de1456c60ad16a8b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 12:48:07 GMT
ADD file:251053dbd1ce0b3744de3eecf53a3ef8ccf92ea509678e59800952c3dbd1b32c in / 
# Fri, 15 May 2020 12:48:09 GMT
CMD ["bash"]
# Sat, 16 May 2020 09:08:28 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 09:08:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 May 2020 09:08:35 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 May 2020 09:09:42 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 09:09:45 GMT
ENV LANG=C.UTF-8
# Sat, 16 May 2020 09:09:46 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 May 2020 09:09:46 GMT
ENV ROS_DISTRO=melodic
# Sat, 16 May 2020 09:09:59 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 May 2020 09:12:45 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 09:12:52 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 May 2020 09:12:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 May 2020 09:12:53 GMT
CMD ["bash"]
# Sat, 16 May 2020 09:14:15 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 09:14:55 GMT
RUN apt-get update && apt-get install -y     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8e144e997aec62ed9c3bb1ff83ae2a62cbea252858abfb48ac60bb2078817a6c`  
		Last Modified: Fri, 15 May 2020 12:55:43 GMT  
		Size: 43.2 MB (43163052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adcea988ace3277be71b815d98bafecfbc3b947df828bbd494e7085e5fb1585`  
		Last Modified: Sat, 16 May 2020 09:21:42 GMT  
		Size: 9.8 MB (9775014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feaa5401dfe7ddb95dcb6de0a4eb7283aa6a2def14cf3340f8e7b9b4730148d2`  
		Last Modified: Sat, 16 May 2020 09:21:39 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e23dc23b7b13d543ecc54f90d6b010b53fa3db276c2f8c57217adf1d89a97c5e`  
		Last Modified: Sat, 16 May 2020 09:21:38 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27290dc07596e678a0735240b71e41a14953d50db4af85a8992c5db289dedf7f`  
		Last Modified: Sat, 16 May 2020 09:21:58 GMT  
		Size: 62.1 MB (62097672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a844380c84bf9a25745c28fd3bac50cf3e8215b708559843d527e3402d87f624`  
		Last Modified: Sat, 16 May 2020 09:21:38 GMT  
		Size: 247.7 KB (247737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81ded023357ea030fbb8a3b72370c16c6d6b20e664b1074159b1d0b05f37850`  
		Last Modified: Sat, 16 May 2020 09:22:46 GMT  
		Size: 230.4 MB (230401736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f15673969bdf41754d0b000c9eb2d6a97266d1c63ef171c362c822d9e86b5b`  
		Last Modified: Sat, 16 May 2020 09:21:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6bc732aa84f09e693b067588e92f67f2bba46a359f79c293a79acb6cb0c6331`  
		Last Modified: Sat, 16 May 2020 09:23:18 GMT  
		Size: 103.0 MB (102958305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8cc0e17e7b4b401e097202ab6b3e58094292346805f92ae85be2ffc44398725`  
		Last Modified: Sat, 16 May 2020 09:23:27 GMT  
		Size: 16.1 MB (16072800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
