## `ros:melodic-ros-core-stretch`

```console
$ docker pull ros@sha256:42e73ae48e0ef8dbbe0c87b47d1122d35f1c2a1a77f46f09d56429dcf423695e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-stretch` - linux; amd64

```console
$ docker pull ros@sha256:0e4d2a0ad1bddb9ca580eccaebef9258c2cf891f02f9f5b44606940b52989933
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.1 MB (322119466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9354e8ea42029350d176adb5113c1d8b4f1ac32d01c35ac2572a261c53beed16`
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

### `ros:melodic-ros-core-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:dd714165f4f553ff40529879a08bf4b97279f2a9cb77b39275368f4fed39139b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.6 MB (274565831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bdbc473f36d5a18d2e94bf4131eea7d09c1e0fcd90142bee30cf1adafb57092`
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
