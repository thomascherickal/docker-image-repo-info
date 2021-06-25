## `gazebo:latest`

```console
$ docker pull gazebo@sha256:5cf2006ed07b171423787e3b36ffe3d37ab27b1a1f6ef597d1890367d7eb7f2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:latest` - linux; amd64

```console
$ docker pull gazebo@sha256:a0bea85908396205adf35ccab373ca162366419d9913b7c0f8ae49a8cdfd7b6d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **603.7 MB (603736794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fc76b704d31e344dd2e74d83129aa506c60b8542cb8531f6a8e049c78be2ee9`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:24:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:24:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:24:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 18 Jun 2021 01:24:42 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Thu, 24 Jun 2021 19:38:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo11=11.6.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 24 Jun 2021 19:38:02 GMT
EXPOSE 11345
# Thu, 24 Jun 2021 19:38:02 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Thu, 24 Jun 2021 19:38:02 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Thu, 24 Jun 2021 19:38:03 GMT
CMD ["gzserver"]
# Thu, 24 Jun 2021 19:43:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     libgazebo11-dev=11.6.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7068ef4db9e492493ff87fbf9095d1e4880263be63a6f42639411a96d5ed57f8`  
		Last Modified: Fri, 18 Jun 2021 02:27:02 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de016a33ce4c52c358d5182933555f132ede796ba07843ea5c1bdb742d9e61a`  
		Last Modified: Thu, 24 Jun 2021 19:46:45 GMT  
		Size: 16.1 MB (16149077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c25740ed17f0991dfd51590656554367fc63d82af01be6cad451d1aaa514ba73`  
		Last Modified: Thu, 24 Jun 2021 19:46:42 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dc1db69196852d66ee41dc90ac9918848d69a11a7a38240dcaf96e3c99074d`  
		Last Modified: Thu, 24 Jun 2021 19:46:42 GMT  
		Size: 5.5 KB (5507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd76b0a40f2b4498ea558773c8591ff6f08414f28e36ebea6634411a77619382`  
		Last Modified: Thu, 24 Jun 2021 19:47:15 GMT  
		Size: 273.2 MB (273223750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aee202d0ec5c345beba96ba5eb4556b91845ffc894e251ca3fd8bfa127e4075`  
		Last Modified: Thu, 24 Jun 2021 19:46:42 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79419d0cab2b63835ff32273bf29458b7e91c47682d1aee96df78f92a262d665`  
		Last Modified: Thu, 24 Jun 2021 19:48:14 GMT  
		Size: 284.6 MB (284620664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
