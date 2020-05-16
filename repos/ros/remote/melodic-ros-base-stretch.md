## `ros:melodic-ros-base-stretch`

```console
$ docker pull ros@sha256:6f218a96f906d55c67d8c8a0112c1b62d000ca22d5e875ed75c98449300d77f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-stretch` - linux; amd64

```console
$ docker pull ros@sha256:b88e0fcc172ad6cb6567486c5cb3ac2a69ecf4ee492a073703412f106b0a27e5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **505.6 MB (505585381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:232a00554a24f65a0da68531b75e050f3268ce08f965ae1a0ba4e694b91c8df3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:33:25 GMT
ADD file:13031623172f5c5857e27de93553adedf17d955fa370882f850bb6ed6fb8cee7 in / 
# Fri, 15 May 2020 06:33:25 GMT
CMD ["bash"]
# Sat, 16 May 2020 03:59:11 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 03:59:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 May 2020 03:59:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 May 2020 04:00:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 04:00:07 GMT
ENV LANG=C.UTF-8
# Sat, 16 May 2020 04:00:07 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 May 2020 04:00:08 GMT
ENV ROS_DISTRO=melodic
# Sat, 16 May 2020 04:00:14 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 May 2020 04:01:52 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 04:01:54 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 16 May 2020 04:01:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 May 2020 04:01:54 GMT
CMD ["bash"]
# Sat, 16 May 2020 04:02:57 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1c6172af85ee14a8db5a3a51d406b768dfa94d196c06d0d06d591507cf8199f0`  
		Last Modified: Fri, 15 May 2020 06:40:31 GMT  
		Size: 45.4 MB (45375207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fda4a46c1d10f88aabb05da22ec1b0b29e36528fa63d6ad5d315eef32b04d0`  
		Last Modified: Sat, 16 May 2020 04:06:33 GMT  
		Size: 10.5 MB (10476838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74529292be06ac11f652a0185d3b8a8e7c8e6318f78145c9fc6a1f62ab665d83`  
		Last Modified: Sat, 16 May 2020 04:06:32 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9068d1ad5bb66c7ce4974550fa3d9bd1a50ddd06b3aff537cf8ac34edf7dbc7b`  
		Last Modified: Sat, 16 May 2020 04:06:30 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2a7091997ccf0c3afb96ac38925f448e86129e61725cd384d216b8db2da380`  
		Last Modified: Sat, 16 May 2020 04:06:47 GMT  
		Size: 64.8 MB (64797298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3728aa494cb44476d46affef19ab460b7bc376333944a5db9eee751da17d8981`  
		Last Modified: Sat, 16 May 2020 04:06:30 GMT  
		Size: 247.7 KB (247672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3892457fe31ca1f052dc113ae893fb097c7f869363701bc2762a648f9547db9e`  
		Last Modified: Sat, 16 May 2020 04:07:20 GMT  
		Size: 276.2 MB (276209403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39976de06deee43924e049833042e4781f041b7fbf3f42687e6e26ae32a2e98d`  
		Last Modified: Sat, 16 May 2020 04:06:29 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec696c745f89d6b37ff9dec480e2f40cf8471a1cbcc62e5cf79f607183ddd46`  
		Last Modified: Sat, 16 May 2020 04:07:44 GMT  
		Size: 108.5 MB (108477140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:72933564cc48bf57b54e2816702e40937b490d4f71ff3e64beb2d92252765470
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.6 MB (448636450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8254326c4a8f06c3e1541e8619b593fc51e99e32baf7fbe25b584cc011edee5d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 23 Apr 2020 00:58:27 GMT
ADD file:4921b222c4914e830c4c018324aed1904bf1526e01493120ddc9c905373b2673 in / 
# Thu, 23 Apr 2020 00:58:29 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 10:19:27 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 10:19:33 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 23 Apr 2020 10:19:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 23 Apr 2020 10:20:59 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 10:21:02 GMT
ENV LANG=C.UTF-8
# Thu, 23 Apr 2020 10:21:03 GMT
ENV LC_ALL=C.UTF-8
# Thu, 23 Apr 2020 10:21:04 GMT
ENV ROS_DISTRO=melodic
# Thu, 23 Apr 2020 10:21:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 23 Apr 2020 10:24:02 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 10:24:13 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 23 Apr 2020 10:24:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 23 Apr 2020 10:24:16 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 10:25:51 GMT
RUN apt-get update && apt-get install -y     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:decabe2933bfe1939dff94ad523be4904c90e7bea69033943dd32f459d115bab`  
		Last Modified: Thu, 23 Apr 2020 01:05:29 GMT  
		Size: 43.2 MB (43159022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b84e9b12c5036e24d270012ffc332ba283c66c65bb1a11c9c36b62ac52c316`  
		Last Modified: Thu, 23 Apr 2020 10:33:34 GMT  
		Size: 9.8 MB (9774901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863092d8428511c061a2c0340a7ec4d93abf5f123245890332e777c71423f808`  
		Last Modified: Thu, 23 Apr 2020 10:33:30 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32b36b14c03269a863c72850458f82fa87b8d312d31a723483b3f5702fdc05a2`  
		Last Modified: Thu, 23 Apr 2020 10:33:28 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2835519f2d237d39236d2dce0f921f1a6dfd9c0631be6c87023f67600d84dcb`  
		Last Modified: Thu, 23 Apr 2020 10:33:48 GMT  
		Size: 62.1 MB (62097551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966f60228a5fb4c85cc691071f60a0fc0154ee013df14567edd599f828c3b6ad`  
		Last Modified: Thu, 23 Apr 2020 10:33:28 GMT  
		Size: 243.1 KB (243119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee00549af9a42e3dd1e9bc8593968eee697343c02e19600216d07d73c9874cc`  
		Last Modified: Thu, 23 Apr 2020 10:34:38 GMT  
		Size: 230.4 MB (230401327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:619c48071b4dbff1dd36122924749c4e683b84b45a23f252dd209bc3f04d4ada`  
		Last Modified: Thu, 23 Apr 2020 10:33:29 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7aa7bc01ef2228d72d31cf584f125210e89f0a44ebdc2eedbcc4226fd48c2f`  
		Last Modified: Thu, 23 Apr 2020 10:35:13 GMT  
		Size: 103.0 MB (102958711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
