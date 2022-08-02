## `gazebo:gzserver9`

```console
$ docker pull gazebo@sha256:7a6d2ec6ebda68d479ef1711f1bcea8cd6e6681cec3d50e8632d15b96e9587d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gazebo:gzserver9` - linux; amd64

```console
$ docker pull gazebo@sha256:3791407d5898c90387e05a75e274a4dd81937a90191a4d393055370bbaf4bfdc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.5 MB (268463318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdf7d0f4cc7da9ce081145c4a9363603da01b86f511a520aa35a5b182ec882c7`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:42 GMT
ADD file:0eb7f0555d03ff4f0755bba2c3d133e68737888f41390c17710f64b70c8e662a in / 
# Tue, 02 Aug 2022 01:30:42 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 12:57:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 19:22:28 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 19:22:30 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Tue, 02 Aug 2022 19:22:30 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Tue, 02 Aug 2022 19:27:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo9=9.19.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 19:27:23 GMT
EXPOSE 11345
# Tue, 02 Aug 2022 19:27:23 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Tue, 02 Aug 2022 19:27:23 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Tue, 02 Aug 2022 19:27:23 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:22c5ef60a68e3fa0bd8df52f48470e836e823434a3bead43e35e87098a0b01fa`  
		Last Modified: Mon, 01 Aug 2022 16:03:08 GMT  
		Size: 26.7 MB (26710270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa6fbe30fbafa2fd890f1a634056fab84382d475fe85716949a1a44cc77f087`  
		Last Modified: Tue, 02 Aug 2022 13:52:33 GMT  
		Size: 839.1 KB (839126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a20a37e68f2ff06e9122f1c4f304cfd163a98b3213537aa90958872adcbba90`  
		Last Modified: Tue, 02 Aug 2022 19:50:39 GMT  
		Size: 14.7 MB (14709005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a37aaaae3cc0de7884c09a5b62982b1761c956b2bb7371f82544e46bb3aa08`  
		Last Modified: Tue, 02 Aug 2022 19:50:36 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d8feed5867be66bfebe1da59e17e7ea2f2bf188ba9f6d03c506f133021e6c1`  
		Last Modified: Tue, 02 Aug 2022 19:50:36 GMT  
		Size: 5.5 KB (5454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7c1b76032efa7194b94ff3a580331a0d1c3bf469bc82ae1c10d570eba45c0f`  
		Last Modified: Tue, 02 Aug 2022 19:51:04 GMT  
		Size: 226.2 MB (226197835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5143058c9dfa5c18e5795d65ceaaa60cf73077456fee1e4d83590d996ebf7d`  
		Last Modified: Tue, 02 Aug 2022 19:50:36 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
