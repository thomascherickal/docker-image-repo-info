## `gazebo:gzserver11-focal`

```console
$ docker pull gazebo@sha256:3c13454fe0f1b4b3e5a1143434174923e6463f753a6b2b2c4bb94dec42df4abc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gazebo:gzserver11-focal` - linux; amd64

```console
$ docker pull gazebo@sha256:7eb852669280012f4a09194416788eb66a8613021d06b17c7c0753c0797c5f8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.9 MB (321935181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad9d5656cadb2e597ae7e822adf19c91fe94386377f216143c51a6f0a5f276c1`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 13:10:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 19:37:01 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 19:37:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Tue, 02 Aug 2022 19:37:03 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Tue, 02 Aug 2022 19:42:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo11=11.11.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 19:42:30 GMT
EXPOSE 11345
# Tue, 02 Aug 2022 19:42:30 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Tue, 02 Aug 2022 19:42:30 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Tue, 02 Aug 2022 19:42:30 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:3b65ec22a9e96affe680712973e88355927506aa3f792ff03330f3a3eb601a98`  
		Last Modified: Tue, 02 Aug 2022 01:31:59 GMT  
		Size: 28.6 MB (28572596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd3f991215ddc16cd6d5839a01c05ba58b96914830f35c25d3d72e0495b053e7`  
		Last Modified: Tue, 02 Aug 2022 13:55:17 GMT  
		Size: 1.2 MB (1181319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f975dc53e94566ecd50c0efbacbcb7ab2dae0d1d21a030aea799fcb49f3c68d`  
		Last Modified: Tue, 02 Aug 2022 19:53:12 GMT  
		Size: 16.2 MB (16177233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025d059902cf14579bcd9256c0121062b3a38c80389b88f6e5cdbac2f8f9bbef`  
		Last Modified: Tue, 02 Aug 2022 19:53:09 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc7dc7b265c734bcd5aa26c356a8a683c548af06e9296c1c77d3aa0c56d49e1`  
		Last Modified: Tue, 02 Aug 2022 19:53:09 GMT  
		Size: 5.5 KB (5500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6e4c614171992dc939c5d9bbceb40390c9f302b293580078f10940f762411d`  
		Last Modified: Tue, 02 Aug 2022 19:53:42 GMT  
		Size: 276.0 MB (275996905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da9129b5de2cdae62d04d981fc908f1ef99b26c092b8ad4fcec600128f479885`  
		Last Modified: Tue, 02 Aug 2022 19:53:09 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
