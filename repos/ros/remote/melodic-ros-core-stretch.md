## `ros:melodic-ros-core-stretch`

```console
$ docker pull ros@sha256:03781a73ae74f59c15b03e131735074c045f82f88755f6a70d9e8fa9dd205e7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-stretch` - linux; amd64

```console
$ docker pull ros@sha256:7ce3a4fd5b33814bc797ebca6fe5a597a3d4060b51c93d7f3e74e30b0bafa28b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.2 MB (322248206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86599a24f6b8fd60cc744400673fe0a0668511e90891b5f34ffad412123ec3a0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:23:13 GMT
ADD file:e1e13145e23f170f2d55444019a2d18a8cecd6209bba9f4295a35632ad53fdde in / 
# Tue, 09 Feb 2021 02:23:14 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 11:24:08 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 11:24:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 09 Feb 2021 11:24:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 09 Feb 2021 11:24:15 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 11:24:15 GMT
ENV LC_ALL=C.UTF-8
# Tue, 09 Feb 2021 11:24:16 GMT
ENV ROS_DISTRO=melodic
# Tue, 09 Feb 2021 11:26:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 11:26:09 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 09 Feb 2021 11:26:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 09 Feb 2021 11:26:09 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:1e987daa2432270bbfaf366f57583c93b48e0ee6c9fe54fe7f4030b84095627f`  
		Last Modified: Tue, 09 Feb 2021 02:29:20 GMT  
		Size: 45.4 MB (45379885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dfef8404fefc17dca87eada52dd07e7bf488497c0c31fea11a60d978da694ad`  
		Last Modified: Tue, 09 Feb 2021 11:41:05 GMT  
		Size: 6.9 MB (6868182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c6e767fccda9923a28109011a5e7fdda7e9f5841c99cc59bee58d437744ceaa`  
		Last Modified: Tue, 09 Feb 2021 11:41:03 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973024f9f826542d72aca896bca3ed1f99093289ca8442460a1d25549bed8bcd`  
		Last Modified: Tue, 09 Feb 2021 11:41:04 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a0b85ea3938d10333f243bfd23c5bed7f06b58b3a5aaaeca4007a5e2b2eb84`  
		Last Modified: Tue, 09 Feb 2021 11:42:10 GMT  
		Size: 270.0 MB (269998323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f36fe789310fd477065fed5386f3d7ac24047a56072617d59131f960a643d88`  
		Last Modified: Tue, 09 Feb 2021 11:41:03 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:79b362e4a0436629fe5e03e3f35cb110da5d50ee720e05a93d5e450e99f0354d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.7 MB (274717765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d72255a31fccc12a4b02b206a4df31f030fcaee0411541482f4c26762f20934a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jan 2021 00:45:18 GMT
ADD file:bc4af94773a01defa7a79adb22199dde2229843dae224d13d3385c522cb71652 in / 
# Tue, 12 Jan 2021 00:45:22 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 16:52:49 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 16:52:55 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 12 Jan 2021 16:52:57 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 12 Jan 2021 16:52:58 GMT
ENV LANG=C.UTF-8
# Tue, 12 Jan 2021 16:52:58 GMT
ENV LC_ALL=C.UTF-8
# Tue, 12 Jan 2021 16:52:59 GMT
ENV ROS_DISTRO=melodic
# Tue, 12 Jan 2021 16:55:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 16:55:42 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 12 Jan 2021 16:55:43 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 12 Jan 2021 16:55:44 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:ec4f0a0f30ab1b4fc2e412a926b8608502de98203ca1994c7916de2017136729`  
		Last Modified: Tue, 12 Jan 2021 00:54:45 GMT  
		Size: 43.2 MB (43177964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e8239a7d8ab4bee604fb1cbe80d3b4626bc8acc2aac57b72c796f1df90dcfc`  
		Last Modified: Tue, 12 Jan 2021 17:19:42 GMT  
		Size: 6.4 MB (6442128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba0c86565e756ed3e4b30d4defdb5a05c4fa9003af196a2339f78ee34d7327a`  
		Last Modified: Tue, 12 Jan 2021 17:19:41 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1b375834829a4e5e0a592407ed74f1602a3d9b06b46e344684c89d9cb32f29`  
		Last Modified: Tue, 12 Jan 2021 17:19:41 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c41b4520c9fa74d7df36a1d382749cb9a1cc38894d750c425a64ba26e1ab86f3`  
		Last Modified: Tue, 12 Jan 2021 17:20:40 GMT  
		Size: 225.1 MB (225095855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac7f1a09c11b17890907dd9234634ee66ce853062cc262bc85d6fa2eff682c80`  
		Last Modified: Tue, 12 Jan 2021 17:19:41 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
