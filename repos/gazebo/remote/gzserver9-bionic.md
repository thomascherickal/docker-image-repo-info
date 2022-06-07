## `gazebo:gzserver9-bionic`

```console
$ docker pull gazebo@sha256:bf58fc170a4fa89eea9bff64dcb6612124ee57996ef069f11355ca984ef5b68f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gazebo:gzserver9-bionic` - linux; amd64

```console
$ docker pull gazebo@sha256:c6a2dba9a608ba888323fc3e77b74a86df213d6d3573da73b9632c4e88270dc1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.4 MB (268427054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcc9379b4198fd2c76dfb2a605992fcee6162fd7db71d0747a3d17b5990eabaf`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:04 GMT
ADD file:40290d9a94ae76c35ab1f57178130ce1c5b976e34a91e77472ecf7e945ab64f9 in / 
# Mon, 06 Jun 2022 22:21:05 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:58:31 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 02:30:02 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 02:30:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Tue, 07 Jun 2022 02:30:04 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Tue, 07 Jun 2022 02:33:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo9=9.19.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 02:33:10 GMT
EXPOSE 11345
# Tue, 07 Jun 2022 02:33:11 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Tue, 07 Jun 2022 02:33:11 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Tue, 07 Jun 2022 02:33:11 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:09db6f815738b9c8f25420c47e093f89abaabaa653f9678587b57e8f4400b5ff`  
		Last Modified: Wed, 01 Jun 2022 21:51:21 GMT  
		Size: 26.7 MB (26711626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5177ec8aa0752191cb3a72f43a3a9259dcaef6c03b51ff91fd9c0fb0f2e45c2`  
		Last Modified: Tue, 07 Jun 2022 01:45:00 GMT  
		Size: 839.2 KB (839230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f30b40bb586a77953c29419e4d15062e6e58b282e85662010dee3a4149bc88`  
		Last Modified: Tue, 07 Jun 2022 02:48:07 GMT  
		Size: 14.7 MB (14710740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4eb10e7bfffcf4d19aa5305f543772250a25ab43092a936b09871ee3b47a8e`  
		Last Modified: Tue, 07 Jun 2022 02:48:04 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32cd4608854ae952456dec2711dd6678fd893bd4a4f1e03553150c95f77371a`  
		Last Modified: Tue, 07 Jun 2022 02:48:04 GMT  
		Size: 5.5 KB (5462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d65e2e1ae0dd41a55be10d1139c818deef31f255844d856b51c230a7a10c90`  
		Last Modified: Tue, 07 Jun 2022 02:48:31 GMT  
		Size: 226.2 MB (226158368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540d2066a86bba851544d69034b0b4639a547c80dcae7467ec09832c1d31297c`  
		Last Modified: Tue, 07 Jun 2022 02:48:04 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
