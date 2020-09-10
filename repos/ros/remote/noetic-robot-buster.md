## `ros:noetic-robot-buster`

```console
$ docker pull ros@sha256:2278700a0e3c2bc85f301210df11e0b1059f95cf26dc50f48049850194728f12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-robot-buster` - linux; amd64

```console
$ docker pull ros@sha256:049d723d73aea50325df8313ecab7f063311befae2f71b7779ad4af44f368db4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.0 MB (484048191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5dd1d03772d82eb6ab069b3c5f03c4688fd4d839ca175876abafdc29bdff188`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 00:22:55 GMT
ADD file:07a6578d6f507bd9c51bdf4fe41402db5dcf3b9fdf51cd4315778c27da1add39 in / 
# Thu, 10 Sep 2020 00:22:55 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 19:28:59 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 19:29:01 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 10 Sep 2020 19:29:01 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 10 Sep 2020 19:29:02 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 19:29:02 GMT
ENV LC_ALL=C.UTF-8
# Thu, 10 Sep 2020 19:29:02 GMT
ENV ROS_DISTRO=noetic
# Thu, 10 Sep 2020 19:30:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 19:30:10 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 10 Sep 2020 19:30:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 10 Sep 2020 19:30:11 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 19:30:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 19:30:55 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 10 Sep 2020 19:31:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 19:31:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:57df1a1f1ad841deaf50c8f662d77e93b4b17af776ed66148116607f9aceffa8`  
		Last Modified: Thu, 10 Sep 2020 00:33:42 GMT  
		Size: 50.4 MB (50395913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399923c486401be50045b0f29c84f4853323f1affa41df16622258e0020ff369`  
		Last Modified: Thu, 10 Sep 2020 19:39:10 GMT  
		Size: 10.9 MB (10889374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b9e949d50923dec18882ab56807dcf92598ce621d132dd3c170ff57e23677d`  
		Last Modified: Thu, 10 Sep 2020 19:39:08 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a58fcd76fabea04c5d0884cba703f43f6d5f18a01242f6e694deb6ccf4486974`  
		Last Modified: Thu, 10 Sep 2020 19:39:08 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded8f54d0a44e4905d100f4f478a53e6ef2646a8f95f02c1eeccfb629df2de3d`  
		Last Modified: Thu, 10 Sep 2020 19:40:12 GMT  
		Size: 238.8 MB (238837297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a645f56df4b12511d5d353cdd1072c50e6dde09b64644e16a79e07e33048402`  
		Last Modified: Thu, 10 Sep 2020 19:39:08 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad5b4e4f45ee63b871c8e1984a221d3bd4af231e5763adf35a67a1d28bf2f83`  
		Last Modified: Thu, 10 Sep 2020 19:40:39 GMT  
		Size: 86.6 MB (86563113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09814c49bcfb8dccb9668b4dfbd67d81e6145a53a0c7ef7bbee887a16aed30e7`  
		Last Modified: Thu, 10 Sep 2020 19:40:17 GMT  
		Size: 224.4 KB (224417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c571ac33029ab6a00ce199508e215ad142a750b94c72c70e444f9299a0701b`  
		Last Modified: Thu, 10 Sep 2020 19:40:36 GMT  
		Size: 76.0 MB (75965762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c27ea5b687c4a36ed755079a30bee0ca2c65848a55ab858f00f4e16ee74f384c`  
		Last Modified: Thu, 10 Sep 2020 19:40:49 GMT  
		Size: 21.2 MB (21170479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:16868e4633e835c700a7d76284764ddda8cec899ab20a1fc1f30374ac8e4890f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **423.6 MB (423618747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c7acc643b1e28e955a454077a7cc6a978913108dc190dba1cf266f28cf9b081`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:50:21 GMT
ADD file:c8c11e622b1b8a1e31f32e2457ff4d1314d5cd4a7ad22b3991ab9d0542db23fd in / 
# Wed, 09 Sep 2020 23:50:22 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 18:07:00 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 18:07:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 10 Sep 2020 18:07:07 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 10 Sep 2020 18:07:09 GMT
ENV LANG=C.UTF-8
# Thu, 10 Sep 2020 18:07:10 GMT
ENV LC_ALL=C.UTF-8
# Thu, 10 Sep 2020 18:07:12 GMT
ENV ROS_DISTRO=noetic
# Thu, 10 Sep 2020 18:11:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 18:12:09 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 10 Sep 2020 18:12:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 10 Sep 2020 18:12:17 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 18:13:46 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 18:14:20 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 10 Sep 2020 18:15:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 18:16:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d3a32671b6316bd11f4bf18cb034394ac94d2bb3bc6d09de388b19b06fb94b91`  
		Last Modified: Wed, 09 Sep 2020 23:58:45 GMT  
		Size: 49.2 MB (49175549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fada41445f002b0de9ef1f01bf1b05aed044cbb407b487db5a5e1352bbda16d`  
		Last Modified: Thu, 10 Sep 2020 18:33:20 GMT  
		Size: 10.9 MB (10881945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eda9628763a567c13b6ffd0c5b79fc235c51103fa9724f14598a3a0e06ef180`  
		Last Modified: Thu, 10 Sep 2020 18:33:16 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd2b7a76d7308a1d2560bca63b7771f0798ece16b3cd1df9c596fca20686592`  
		Last Modified: Thu, 10 Sep 2020 18:33:15 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15dd71827aa7b3a011f910eecfe88aacbe135cae512a657976fdf9dbaf1dea8`  
		Last Modified: Thu, 10 Sep 2020 18:34:19 GMT  
		Size: 184.1 MB (184073881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ddc38cd48b4e686de79d8ff245c8b7ffd578bcfd845d6e4f33b043f826bb36`  
		Last Modified: Thu, 10 Sep 2020 18:33:15 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31cc61790a22052687e1a3883fde6f9ee45a7bc98021a2998b93e2befce29beb`  
		Last Modified: Thu, 10 Sep 2020 18:34:46 GMT  
		Size: 84.4 MB (84355549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211a09c9e39609d1ec9adc086f9f8d2cdd69fd7e46f0d6f98181a19730ce8dc0`  
		Last Modified: Thu, 10 Sep 2020 18:34:28 GMT  
		Size: 224.5 KB (224473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb1ef5f83a4daae14ff5664ae2b9b86c52eb5e79b04c64240c1e477ce359825`  
		Last Modified: Thu, 10 Sep 2020 18:34:46 GMT  
		Size: 74.1 MB (74089936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d5212463de83084b75fd6e07c0358461d3f1e60a4bb14cfcb92d35c3a48029`  
		Last Modified: Thu, 10 Sep 2020 18:34:58 GMT  
		Size: 20.8 MB (20815577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
