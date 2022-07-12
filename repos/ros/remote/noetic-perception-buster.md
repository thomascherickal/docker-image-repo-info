## `ros:noetic-perception-buster`

```console
$ docker pull ros@sha256:e479a3ce3043dc06d81fa2ea090e0c2d432be801e31c4baac795843702e9ef16
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-perception-buster` - linux; amd64

```console
$ docker pull ros@sha256:eb9cb9d2843ef50aa96edfc64d29690882633227d956698d9b99643ff211ff89
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **951.5 MB (951527328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb871071aeb60fde83497f6af89ca97c419468b44cbdd3bbc6f97b33140c1a98`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:36 GMT
ADD file:2f32dd3ef1e51a4d2d6dcf55fbf766434df5b3ada802b087d5761f2fa0cdebf5 in / 
# Thu, 23 Jun 2022 00:20:36 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 12:48:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 12:48:07 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 23 Jun 2022 12:48:09 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 23 Jun 2022 12:48:09 GMT
ENV LANG=C.UTF-8
# Thu, 23 Jun 2022 12:48:09 GMT
ENV LC_ALL=C.UTF-8
# Thu, 23 Jun 2022 12:48:09 GMT
ENV ROS_DISTRO=noetic
# Thu, 23 Jun 2022 12:49:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 11 Jul 2022 23:38:10 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Mon, 11 Jul 2022 23:38:10 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 11 Jul 2022 23:38:10 GMT
CMD ["bash"]
# Mon, 11 Jul 2022 23:38:32 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Mon, 11 Jul 2022 23:38:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 11 Jul 2022 23:39:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 11 Jul 2022 23:41:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ea267e4631a981caf2841a7e9a1faf29cef9d020c4378fc64845802d17586531`  
		Last Modified: Thu, 23 Jun 2022 00:25:38 GMT  
		Size: 50.4 MB (50440811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d614310471c61e4200046b8f7adea9e8513871ad4fde9b669e49cafd656bde2`  
		Last Modified: Thu, 23 Jun 2022 12:53:58 GMT  
		Size: 10.9 MB (10892280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c90706f4c8a053c5c76e44d43756ced985189146b36ac63497e25ceceefc5c5`  
		Last Modified: Thu, 23 Jun 2022 12:53:57 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832307bf10c44d39b4524638f32d96d980cbea1925cc229df4ca7c97c3d08e81`  
		Last Modified: Thu, 23 Jun 2022 12:53:57 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09580d323567b8cc4622a787e2540c618939571a6ba340dd72e42597029cbba5`  
		Last Modified: Thu, 23 Jun 2022 12:54:29 GMT  
		Size: 239.2 MB (239166199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39dada285349dd73a05a5efcc9f7a78ece2b4d3f8af94032d497caeef5a9f16`  
		Last Modified: Tue, 12 Jul 2022 00:04:53 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c4c45b18027d32f13d3a3054125f1bc02100af05c5625dcaffaeb925a75d49d`  
		Last Modified: Tue, 12 Jul 2022 00:05:12 GMT  
		Size: 86.7 MB (86716172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:425afd918406f89360e651fe6438c7d56e07c3373139984762889c163123ca25`  
		Last Modified: Tue, 12 Jul 2022 00:04:59 GMT  
		Size: 316.4 KB (316435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04828242e79a3ae204a877e305d8dcdce6cdbd7e2f94d828405673f5c3c860ed`  
		Last Modified: Tue, 12 Jul 2022 00:05:10 GMT  
		Size: 76.0 MB (75977435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267a37db93cbe4ea7c084703d2d858f8589905137999a3aa638cacab21060fc1`  
		Last Modified: Tue, 12 Jul 2022 00:06:45 GMT  
		Size: 488.0 MB (488015586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:1c735db133c7474320989e3323eee02d48925994e5046b6ded44b1e5fa625506
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **867.8 MB (867793498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c3143db01c257625641f6e99ec68e62dbf02c888747af3f399297a222722752`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:54 GMT
ADD file:a5e3c0ffa9f9754a6d77fafd8288e699a70f7f6ff7c5912a065f1c69f1393e99 in / 
# Thu, 23 Jun 2022 00:40:55 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 13:15:38 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 13:15:39 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 23 Jun 2022 13:15:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 23 Jun 2022 13:15:41 GMT
ENV LANG=C.UTF-8
# Thu, 23 Jun 2022 13:15:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 23 Jun 2022 13:15:43 GMT
ENV ROS_DISTRO=noetic
# Thu, 23 Jun 2022 13:16:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 11 Jul 2022 23:51:37 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Mon, 11 Jul 2022 23:51:39 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 11 Jul 2022 23:51:40 GMT
CMD ["bash"]
# Mon, 11 Jul 2022 23:52:05 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Mon, 11 Jul 2022 23:52:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 11 Jul 2022 23:53:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 11 Jul 2022 23:56:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8d6f1451981514e25c21542f5c7ee9bb90052b8856b484ce47294cbf1fd5a234`  
		Last Modified: Thu, 23 Jun 2022 00:47:46 GMT  
		Size: 49.2 MB (49229092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbcd1485b8f3c07588c4ea63df43ce191dc4bd704f4db66afbba5befa84a13c3`  
		Last Modified: Thu, 23 Jun 2022 13:24:26 GMT  
		Size: 10.7 MB (10688303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a806e582281d47bb169333c62fc3d5d3d9478b1b26ec2c797fde052f7e0e3d2c`  
		Last Modified: Thu, 23 Jun 2022 13:24:25 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be161c8e6aa95e3bf58f9376749c867ab58036e812be1274d6a856816a5f07e5`  
		Last Modified: Thu, 23 Jun 2022 13:24:25 GMT  
		Size: 1.9 KB (1947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba910dea9270aeab8bd65e0a16c91c62e0b2be0bae0732297f397d380a67c9a9`  
		Last Modified: Thu, 23 Jun 2022 13:24:55 GMT  
		Size: 184.4 MB (184373444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07abc8cb8cf03a55ac67f13598dc64216c3f7d3b714cb76227e34503975021fe`  
		Last Modified: Tue, 12 Jul 2022 00:14:36 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb51800d2731625f8ee7dea42b44799325ca057a89fa2fa8ba4095d9fab6a4d`  
		Last Modified: Tue, 12 Jul 2022 00:14:56 GMT  
		Size: 84.5 MB (84500931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f3a213cb43d539fd29a7ec031bd8e7a5c8ebebb57fcc228537bb39e09e622b`  
		Last Modified: Tue, 12 Jul 2022 00:14:44 GMT  
		Size: 316.4 KB (316391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc1edd1228ff9a5e3174f1093cfc400973af026fe7250c62af78c2f8631df3a`  
		Last Modified: Tue, 12 Jul 2022 00:14:54 GMT  
		Size: 73.9 MB (73865033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497a759257b90f202369978538c3f87102a2a617cd514902c5ef319d0b452dd2`  
		Last Modified: Tue, 12 Jul 2022 00:16:22 GMT  
		Size: 464.8 MB (464817934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
