## `ros:galactic-ros1-bridge`

```console
$ docker pull ros@sha256:231822831ea43a77ba490022891e8dd8bde9bda6968da8e2fad3c9203c6f30a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros1-bridge` - linux; amd64

```console
$ docker pull ros@sha256:02e7959fe79dffbe5a7a2b64daa8517ca659f10112e56636c4860e009370d034
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.8 MB (330806483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0a48b04abf6255fa8c8e56e9aa96c21acbd363eb70966dde6fa92ada5040eaa`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:39:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:00:47 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:11:21 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 30 Apr 2022 02:11:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 30 Apr 2022 02:11:22 GMT
ENV LANG=C.UTF-8
# Sat, 30 Apr 2022 02:11:22 GMT
ENV LC_ALL=C.UTF-8
# Sat, 30 Apr 2022 02:14:07 GMT
ENV ROS_DISTRO=galactic
# Sat, 30 Apr 2022 02:14:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:14:52 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 30 Apr 2022 02:14:52 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 30 Apr 2022 02:14:52 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 02:15:13 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:15:19 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 30 Apr 2022 02:15:22 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 30 Apr 2022 02:15:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:15:43 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 30 Apr 2022 02:15:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 30 Apr 2022 02:15:45 GMT
ENV ROS1_DISTRO=noetic
# Sat, 30 Apr 2022 02:15:45 GMT
ENV ROS2_DISTRO=galactic
# Sat, 30 Apr 2022 02:16:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:16:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:16:19 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca43c78a9071a3a99b9aa1fe030cf8ba61c96fbf0b12adc1a85163d395cc10a1`  
		Last Modified: Sat, 30 Apr 2022 00:50:22 GMT  
		Size: 1.2 MB (1180884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695af473b1cd9e144d20d270ac7db7c1e34126fdb27db717ef1b82d4ea459397`  
		Last Modified: Sat, 30 Apr 2022 02:23:44 GMT  
		Size: 5.5 MB (5546712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ecbdd5d86aa1bccfbc93111261e6b9ae8bbd5777bcb704b395d81b82a8e6f7`  
		Last Modified: Sat, 30 Apr 2022 02:26:24 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184a755bf529bfea3fdd27ac8aa0a2c242d828fd03aa912766c514f925b0d324`  
		Last Modified: Sat, 30 Apr 2022 02:26:24 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dab9ed6bab5f87837f781c6b6f2631af5cec9d24316a3d8af71d7971b5cf951`  
		Last Modified: Sat, 30 Apr 2022 02:28:04 GMT  
		Size: 103.7 MB (103664283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b8f626b8252407df6df973634a2e4356aa55d4b99b403854f663776c11ff2c`  
		Last Modified: Sat, 30 Apr 2022 02:27:47 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97bb570914f7aa1b5ec420f6cbf026ba7322fc64c3c5031122e00c84b1d24ca7`  
		Last Modified: Sat, 30 Apr 2022 02:28:25 GMT  
		Size: 74.5 MB (74496458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03cf4960f48abacca0ac88e2b9be02b38222978d892ba3aa43d75f87c217f0fb`  
		Last Modified: Sat, 30 Apr 2022 02:28:14 GMT  
		Size: 263.0 KB (262991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889790d3bdef1e28cfa5d700256863193afa101836f0bd7dc9e8e6edd29c42bf`  
		Last Modified: Sat, 30 Apr 2022 02:28:14 GMT  
		Size: 2.2 KB (2216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f949686274ec16d939a0de3707aca670ade11bef3549b9869a715869dac0f5e0`  
		Last Modified: Sat, 30 Apr 2022 02:28:18 GMT  
		Size: 22.1 MB (22113734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e36b076d3c432c32a1b72ee2acef202c45bb3a1129dc73bafb1709f91aa40a8`  
		Last Modified: Sat, 30 Apr 2022 02:28:38 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77e328c99e65115ff1d3acbbb4cad40c0d9324e8e313e69534f935bd5b98975`  
		Last Modified: Sat, 30 Apr 2022 02:28:38 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074b9d4fcd07ae71c51c4607009e0593b3eb13d9636f7fd9d67bd7e0259a715b`  
		Last Modified: Sat, 30 Apr 2022 02:28:53 GMT  
		Size: 78.6 MB (78599045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7880ae899fe2926cd0e88e72b3b6f2de282201480b8588750b8115cdb87f60b7`  
		Last Modified: Sat, 30 Apr 2022 02:28:42 GMT  
		Size: 16.4 MB (16370893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750fe75e312bcc6b30e34803c5381594d679cfbe3ab4076624bbd36e5c53816e`  
		Last Modified: Sat, 30 Apr 2022 02:28:38 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros1-bridge` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:48962fe4314d31cfbe0c476bc5fc5aa5c6e3a86b036d2529e4181ccf4f3f6d02
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.0 MB (318030674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cce0a6ba85ea8984ccfe00e891f3fa1fc5714370e4d0d173729d06d89ead5597`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:20:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:20:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:25:50 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Sat, 30 Apr 2022 00:25:52 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 30 Apr 2022 00:25:53 GMT
ENV LANG=C.UTF-8
# Sat, 30 Apr 2022 00:25:54 GMT
ENV LC_ALL=C.UTF-8
# Sat, 30 Apr 2022 00:29:05 GMT
ENV ROS_DISTRO=galactic
# Sat, 30 Apr 2022 00:29:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:29:55 GMT
COPY file:57f71198b74c2c1967889acdfddb85d428137580d18be4211971fc7381557b6c in / 
# Sat, 30 Apr 2022 00:29:56 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 30 Apr 2022 00:29:57 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:30:29 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:30:34 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 30 Apr 2022 00:30:37 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Sat, 30 Apr 2022 00:30:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-base=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:31:09 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 30 Apr 2022 00:31:12 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 30 Apr 2022 00:31:13 GMT
ENV ROS1_DISTRO=noetic
# Sat, 30 Apr 2022 00:31:14 GMT
ENV ROS2_DISTRO=galactic
# Sat, 30 Apr 2022 00:31:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-comm=1.15.14-1*     ros-noetic-roscpp-tutorials=0.10.2-1*     ros-noetic-rospy-tutorials=0.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:31:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros1-bridge=0.10.1-2*     ros-galactic-demo-nodes-cpp=0.14.3-1*     ros-galactic-demo-nodes-py=0.14.3-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:32:01 GMT
COPY file:f2fca591c0e2a31379c7ea28a9948ef5ee9d4a95b4831016253c1ef1a4f39718 in / 
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2837428b54ca227343b28e2aebf5f943eb61317acb706203bbd53ccd36b1faa`  
		Last Modified: Sat, 30 Apr 2022 00:38:20 GMT  
		Size: 1.2 MB (1182149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782caaf301f52c6f48c207e662cbaff846f5e221ff2d301aa5123d59be9f9cdc`  
		Last Modified: Sat, 30 Apr 2022 00:38:18 GMT  
		Size: 5.3 MB (5321931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e518f0b96ea742e65f2524920ef0978594bec0e17d20b42b1068bfc73720bd`  
		Last Modified: Sat, 30 Apr 2022 00:41:03 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be28b19174686f17ae1317ae4d3c9000a0c5da2daba3797916241b4eff9b024e`  
		Last Modified: Sat, 30 Apr 2022 00:41:03 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc429bf8652d7c199bc2696f50eb5d6d96995a020de7042fcefc0c861e53b494`  
		Last Modified: Sat, 30 Apr 2022 00:42:49 GMT  
		Size: 100.0 MB (100040496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24d376e5e7a9471996a0ba2517b9f4860601c4b261f5b4568a13a3138e91451`  
		Last Modified: Sat, 30 Apr 2022 00:42:32 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c48e7d9d49e9d72193ee8a2410040fc2dbb905e90a5e87a2963ec1efc64dc2`  
		Last Modified: Sat, 30 Apr 2022 00:43:11 GMT  
		Size: 68.6 MB (68617962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61d3c508c87335df6c90cdb63cfc533f43c7e76223a40d60d51d5a56d650b11`  
		Last Modified: Sat, 30 Apr 2022 00:43:01 GMT  
		Size: 262.9 KB (262931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:174ce5304359afaff45591ca5d498cc4399f317742522047929ffc39f06c6af2`  
		Last Modified: Sat, 30 Apr 2022 00:43:01 GMT  
		Size: 2.1 KB (2106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb658821f56c3fbaa2fa5ca66ecb34a323faf00bb9654441fcc020fd19e8570f`  
		Last Modified: Sat, 30 Apr 2022 00:43:04 GMT  
		Size: 21.4 MB (21435249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c02c9a7a06776ddd2eac23260813a366f1d3f3e7dc80e9a4d2f2f6b4dbf53e63`  
		Last Modified: Sat, 30 Apr 2022 00:43:27 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41cb6af35ed1d38b83eeb5f73eb9a821e0d2bb870d66062baff249aee9ecddb2`  
		Last Modified: Sat, 30 Apr 2022 00:43:43 GMT  
		Size: 78.3 MB (78325638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44cd3ad1141d2aec27411320026308bd67afff55754028e3c0c53d04a45846d8`  
		Last Modified: Sat, 30 Apr 2022 00:43:30 GMT  
		Size: 15.7 MB (15669988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a8c3f4e5657b2b41897151effdbe5aa3f29312c704a85e9612296bc5996335`  
		Last Modified: Sat, 30 Apr 2022 00:43:28 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
