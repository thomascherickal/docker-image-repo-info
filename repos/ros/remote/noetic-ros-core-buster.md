## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:1ef4106be6a8e420cb55f03ee4ffc0cdad45109ac0a8cca4534263c7568c202d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:a7af5be0e69b6a584496422fdbe9e44f90b40520df8a14e087a8218967385027
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.2 MB (300211143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b52a9050b0e06f97b9af2b7f92c3333edb130b7cc8abf1245525ba694d09873c`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:36 GMT
ADD file:53e587afdbeaee60cc14bd95907f14c8303c04b98c72f98e2c54d4343f15dd38 in / 
# Tue, 12 Jan 2021 00:32:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:08:45 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:08:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 12 Jan 2021 01:08:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 12 Jan 2021 01:08:48 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 01:08:48 GMT
ENV LC_ALL=C.UTF-8
# Tue, 12 Jan 2021 01:08:48 GMT
ENV ROS_DISTRO=noetic
# Tue, 12 Jan 2021 01:10:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:10:26 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 12 Jan 2021 01:10:27 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 12 Jan 2021 01:10:27 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:b9a857cbf04d2c0d2f0f6b73e894b20a977a6d3b6edd9e27d080e03142954950`  
		Last Modified: Tue, 12 Jan 2021 00:38:49 GMT  
		Size: 50.4 MB (50399171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d472a295ebd41d3968f8d863e1015d367c18e985c1c0f56d543463857ec9647e`  
		Last Modified: Tue, 12 Jan 2021 01:24:06 GMT  
		Size: 10.9 MB (10890313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d374fcbac4a1edeece11e802c028e58bcfd68f594a873fe3daa75cb39560a5a`  
		Last Modified: Tue, 12 Jan 2021 01:24:02 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82e0241a79b24e9ee7ee6f9df3d32a58e6a527c754d734ffdeab34eb9f7d189`  
		Last Modified: Tue, 12 Jan 2021 01:24:03 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090f94ca05cb3b6e59c6c7edda6c987adc2e22ba0327be09a7d9209b23653182`  
		Last Modified: Tue, 12 Jan 2021 01:25:15 GMT  
		Size: 238.9 MB (238919824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a4f8987d94cbf12fbebd2ede2b2e65b75267777ba507219d725e88a9a5cb21`  
		Last Modified: Tue, 12 Jan 2021 01:24:03 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:8fc5a63cfb8e9777d2c94c0cab1c70027b788863d16ef7648872a51c231ef83e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.2 MB (244210979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fc2d256194b2b1695bdbd420657b89a4a0221c2ae871caa923bd1afd18480c7`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:23 GMT
ADD file:b08f373022952dba7d08b7fc02909d9e369c9727e0e4f62d6110e41e70e668cc in / 
# Fri, 11 Dec 2020 02:45:25 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 23:25:05 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 23:25:09 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 11 Dec 2020 23:25:11 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 11 Dec 2020 23:25:11 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 23:25:13 GMT
ENV LC_ALL=C.UTF-8
# Fri, 11 Dec 2020 23:25:14 GMT
ENV ROS_DISTRO=noetic
# Fri, 11 Dec 2020 23:27:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 23:27:34 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 11 Dec 2020 23:27:35 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 11 Dec 2020 23:27:36 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:99e5136f81cd2a8cc226c42435d6f4f30584d168cc51f4d4afd2d5611e4d2215`  
		Last Modified: Fri, 11 Dec 2020 02:52:45 GMT  
		Size: 49.2 MB (49180317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6802a596e847ecc40fc64a4020bce9c6b7ec241a9a0adff6a2f4b93c30b2144`  
		Last Modified: Fri, 11 Dec 2020 23:41:10 GMT  
		Size: 10.9 MB (10882958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d048a0e9c93d12fc2502ef2bd5aff74d265481bfe6a09ed85acc1b9d28d689`  
		Last Modified: Fri, 11 Dec 2020 23:41:07 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89503d24c7d28733c7447800ad677d2131c8d16d0a168ebb554b2b3daaf1a1f1`  
		Last Modified: Fri, 11 Dec 2020 23:41:07 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:215ec51670c89e647b8382b61d566bad5238b2661b6575cae78036b6dbc1da44`  
		Last Modified: Fri, 11 Dec 2020 23:42:01 GMT  
		Size: 184.1 MB (184145865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f19aa0624291920427cd6503ba38ebd048f0d00f4e6f303a9893c73a1d212a`  
		Last Modified: Fri, 11 Dec 2020 23:41:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
