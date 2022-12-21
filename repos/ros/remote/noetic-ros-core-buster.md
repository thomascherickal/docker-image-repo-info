## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:ff12e51a96381a0c7c34fa5dbcbb911a0e441533f2e675b13fc500709a18bd62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:89966fc74ab3551a125b04fea2b7fd1297c887e1b75c7300db89c9e5dd13468f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300553687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d777c39d82dfc632fbaf4792c635130dab511f386c4f9762ca82386a8ac32832`
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

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:10a4a8ca5f47bf3af732cfd6eedd0cc97e8dfb0478a5254bf23562b2bbbee66a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.5 MB (244527099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:854b760e1ee2468a1f009aac750b3f18b0d69c1e7f88efc93a0e51d8e0a4ea91`
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
