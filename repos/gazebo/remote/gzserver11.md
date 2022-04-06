## `gazebo:gzserver11`

```console
$ docker pull gazebo@sha256:0d4ffbcd80c643cf967e32f2e89f05e44189bc793e1d93f5f86167c5f6ddc8f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gazebo:gzserver11` - linux; amd64

```console
$ docker pull gazebo@sha256:874bddc2f0a8e7f4642055d646ec9b111e5c7583983774184b46a00bd0d8e7b2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.8 MB (321780811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c87bf13faa785d3ced0dc623a6938f850a351b3c04e06af9654e3c6192cf4bd7`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Tue, 05 Apr 2022 22:20:50 GMT
ADD file:b83df51ab7caf8a4dc35f730f5a18a59403300c59eecae4cf5779cba0f6fda6e in / 
# Tue, 05 Apr 2022 22:20:51 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 23:50:43 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:51:09 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:51:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Tue, 05 Apr 2022 23:51:11 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Tue, 05 Apr 2022 23:54:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo11=11.10.2-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:54:18 GMT
EXPOSE 11345
# Tue, 05 Apr 2022 23:54:18 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Tue, 05 Apr 2022 23:54:19 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Tue, 05 Apr 2022 23:54:19 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:e0b25ef516347a097d75f8aea6bc0f42a4e8e70b057e84d85098d51f96d458f9`  
		Last Modified: Tue, 05 Apr 2022 13:14:03 GMT  
		Size: 28.6 MB (28566292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dbdf8d1aa53ac931cb020f1ee4ae35afbc9afcf41aa966fed51bc2848d19d4c`  
		Last Modified: Wed, 06 Apr 2022 00:01:59 GMT  
		Size: 1.2 MB (1180816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7643321c46f58d98351068533e061c1a058ff43178c3341d17ba3a939c2f0fdb`  
		Last Modified: Wed, 06 Apr 2022 00:02:02 GMT  
		Size: 16.2 MB (16169898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148eaf4ebefa3d433d143cb7c18a888abbf3737a558ae718570d538e7497d91e`  
		Last Modified: Wed, 06 Apr 2022 00:01:56 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803359cbbf028b7a41a457abc99e539c7810a645230d7a07da244ba83e14bd57`  
		Last Modified: Wed, 06 Apr 2022 00:01:56 GMT  
		Size: 5.5 KB (5496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eedc7558b49301df4c075d8be531fbd5462aa9d2afa5ed5384db9940920f1843`  
		Last Modified: Wed, 06 Apr 2022 00:02:29 GMT  
		Size: 275.9 MB (275856684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7d68c47db4776d04402e814b5d371a3252539295139e3db2acf9715893f71f`  
		Last Modified: Wed, 06 Apr 2022 00:01:56 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
