## `gazebo:gzserver9`

```console
$ docker pull gazebo@sha256:e5ffae311500cf0fbcecba2e76ad8b87efabb400c3ed392c91d897bca9b66bd2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gazebo:gzserver9` - linux; amd64

```console
$ docker pull gazebo@sha256:216c4ea494fa9674bc054b07c070f418cb0542e736097f28e158c387faabdccd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.5 MB (268455636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd26253029b85ba449d9397d607c2042fa9166d933669c583cfb1baa998f19dc`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:18 GMT
ADD file:8b379a8fd96e76d10db6f9ae4e9675de33d227db0431ca2a7ca799119e905e8f in / 
# Thu, 01 Sep 2022 23:46:18 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:55:19 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:55:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:55:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 02 Sep 2022 02:55:31 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 02 Sep 2022 02:58:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo9=9.19.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:58:05 GMT
EXPOSE 11345
# Fri, 02 Sep 2022 02:58:05 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 02 Sep 2022 02:58:05 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 02 Sep 2022 02:58:05 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:dad0f37c70a668d101c86b5c769d452ff29c6d51f811891384cc7da00fce192f`  
		Last Modified: Wed, 31 Aug 2022 06:57:55 GMT  
		Size: 26.7 MB (26710085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210c2da7b10ffa6d0e2b3a3af917a40d5b42b1606cf3aff1dbbd48b1da768dd2`  
		Last Modified: Fri, 02 Sep 2022 03:13:02 GMT  
		Size: 831.0 KB (830989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c2f193a51cd0afec561c749fe8ca94db1dbd5dd0889044530e2e627ea87d63`  
		Last Modified: Fri, 02 Sep 2022 03:13:02 GMT  
		Size: 14.7 MB (14709235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364bd7888a65fc5650010670936211e76efef4b32bb6316216e3a86d40c69e2b`  
		Last Modified: Fri, 02 Sep 2022 03:12:59 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abadb91965c06a226e79402d88cba56f1c093e69450135088903042cfe9da2a7`  
		Last Modified: Fri, 02 Sep 2022 03:12:59 GMT  
		Size: 5.5 KB (5460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3967e5d56041a046ad1ac4b5c9304a874129682d72d7bcb32d700cc8803a545e`  
		Last Modified: Fri, 02 Sep 2022 03:13:26 GMT  
		Size: 226.2 MB (226198240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee746f0daf26092d7c4c23483f55d4e94625c80aafb6f9ad33a0ec39fa7a2691`  
		Last Modified: Fri, 02 Sep 2022 03:12:59 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
