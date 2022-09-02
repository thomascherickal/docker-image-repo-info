## `ros:rolling-ros-base`

```console
$ docker pull ros@sha256:e1b81803e71c64f9fb4a9465103d7d6e26acaf114ce724bca30ffda6a49bc521
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:rolling-ros-base` - linux; amd64

```console
$ docker pull ros@sha256:7b4c586e54c27743aab2a47e40c9703663d5a9e8de1e08173aafbce70150359c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.0 MB (262952620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:223af4769b7faa40e705248499c92752b2b8291256bf897cda3f27d405b0fe59`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 04:47:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:43 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 04:47:44 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 04:47:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 04:47:45 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 04:47:45 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 04:59:53 GMT
ENV ROS_DISTRO=rolling
# Fri, 02 Sep 2022 05:00:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:00:33 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 05:00:33 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 05:00:33 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 05:00:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 05:01:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 05:01:07 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 05:01:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3547d30662b8f49979ed975e15692a70c7bb853c6f802402d13fae5baf9c98`  
		Last Modified: Fri, 02 Sep 2022 05:11:58 GMT  
		Size: 1.2 MB (1175731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e2de4e9186b2154434f8288f5aa7bb8a9d6dc013e0874f7f022b8ae24dfbf0`  
		Last Modified: Fri, 02 Sep 2022 05:11:56 GMT  
		Size: 3.8 MB (3827460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a3a3add45c3c8843eaf042b57f390470bedeb0ac07a77f9c6612bef030c530`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47468e731ca16770a971f055794d9d4098fc38d48dd35c9031b3076ca342047`  
		Last Modified: Fri, 02 Sep 2022 05:11:55 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3dc50070b191638388b8a6f45838ba98380554ae338b31cc128a05d2395988`  
		Last Modified: Fri, 02 Sep 2022 05:14:57 GMT  
		Size: 106.2 MB (106166428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd81258fb9cb69dfc99169ad3cb6e4fdf405255a94947c3080addd04660088d9`  
		Last Modified: Fri, 02 Sep 2022 05:14:39 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06230df102e423df05671bcf3524ba4a66b7948f791b968310ce88c3912d891b`  
		Last Modified: Fri, 02 Sep 2022 05:15:20 GMT  
		Size: 97.8 MB (97849361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fba9b08f3c34427866a17b95897c2bbf6d0ddaa0388e56fec786cc5e8b03e9`  
		Last Modified: Fri, 02 Sep 2022 05:15:07 GMT  
		Size: 280.9 KB (280936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8408c6380a2368a7fad097e912751c17f613c5e60923c6797b34c7146889011c`  
		Last Modified: Fri, 02 Sep 2022 05:15:06 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd491e285c840733c080cbbbbaaff463949c9101c61e114e1827f6c8bcac997`  
		Last Modified: Fri, 02 Sep 2022 05:15:10 GMT  
		Size: 23.2 MB (23221130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:rolling-ros-base` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a9dcdf82e957bea076149139b3c6cdee66559f489613daa7903b56685f7f1aef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.2 MB (255169056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e9bd1d5dd1b3a26db2b810ff05f70c5869229f070eb096aab27f1e691324200`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:15:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:54 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:15:55 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu jammy main" > /etc/apt/sources.list.d/ros2-latest.list
# Fri, 02 Sep 2022 06:15:57 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 02 Sep 2022 06:15:58 GMT
ENV LANG=C.UTF-8
# Fri, 02 Sep 2022 06:15:59 GMT
ENV LC_ALL=C.UTF-8
# Fri, 02 Sep 2022 06:20:47 GMT
ENV ROS_DISTRO=rolling
# Fri, 02 Sep 2022 06:21:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-core=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:21:36 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Fri, 02 Sep 2022 06:21:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 02 Sep 2022 06:21:38 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:22:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 06:22:16 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 02 Sep 2022 06:22:19 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Fri, 02 Sep 2022 06:22:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-rolling-ros-base=0.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81e8a90c277865b9fe52db2db44bfadc7b4a5b90c6e35f9ff56b0949e79f9a9`  
		Last Modified: Fri, 02 Sep 2022 06:34:29 GMT  
		Size: 1.2 MB (1177947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d06c25b67bbbdda5958c2b397a6a9868ac31ba8a8adf79f16a867441aaf6339`  
		Last Modified: Fri, 02 Sep 2022 06:34:27 GMT  
		Size: 3.6 MB (3594798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ae3c2eb3de8889d4850076f921c47d4392ed652c6c949e8bbd1934fa565a93`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755bc2feb97c1316b5973891dbae4001df11b9f157554abbfac9b81d446cbd52`  
		Last Modified: Fri, 02 Sep 2022 06:34:26 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57709850deb7ebb6da7e7913dd7f347b87d4aff6128c1297029b1764763a4c43`  
		Last Modified: Fri, 02 Sep 2022 06:37:27 GMT  
		Size: 103.9 MB (103880245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba67b53a682dfe82f8a87e67d34d26e3a50eacc3e0bf38649a8b67d96c7e03ea`  
		Last Modified: Fri, 02 Sep 2022 06:37:10 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2a782d281bb90dd26f42ed3113a1e4d736c784ad27b4546669bca780ad66bd`  
		Last Modified: Fri, 02 Sep 2022 06:37:51 GMT  
		Size: 95.2 MB (95213961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf639d3046819cf6b3d082dad590518137fc54d4a308acc8f6545b8bb68ac366`  
		Last Modified: Fri, 02 Sep 2022 06:37:38 GMT  
		Size: 280.9 KB (280888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f896ae4cec7dae8bae24fa69bc7c65810575491c2df60e45eebffad0fe8a61bb`  
		Last Modified: Fri, 02 Sep 2022 06:37:38 GMT  
		Size: 2.4 KB (2355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819335435c465f7b44fe0db81c9fddd471a57234896c5daf09af9efb60a54319`  
		Last Modified: Fri, 02 Sep 2022 06:37:41 GMT  
		Size: 22.6 MB (22635152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
