## `gazebo:gzserver11`

```console
$ docker pull gazebo@sha256:030f37ba660faa4218620a0df1ca1f19588ab84ee6aabd04c675322fb6864c83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gazebo:gzserver11` - linux; amd64

```console
$ docker pull gazebo@sha256:1087618dbe2b2c5615a028d988a2b44595e770fe570b5d7ce126fce3ec82940e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.0 MB (322026884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:342fa40fae2fdf7942d6342dd5bb7faa4c43dd73a28233782a3ff2f0a3dcfcf6`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 02:44:48 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 02:45:33 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 02:45:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Thu, 03 Aug 2023 02:45:34 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Tue, 10 Oct 2023 20:25:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo11=11.14.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 10 Oct 2023 20:25:03 GMT
EXPOSE 11345
# Tue, 10 Oct 2023 20:25:03 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Tue, 10 Oct 2023 20:25:04 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Tue, 10 Oct 2023 20:25:04 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aab22f0326d7d89686f4eebe2ba52f86ca4e83a4c69d66dfe4f2b1494eae439`  
		Last Modified: Thu, 03 Aug 2023 02:53:09 GMT  
		Size: 1.2 MB (1198625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7537a4633286752d5bbe02fb22f93fc43f5d85fab59ced7194b862896ac1d1d`  
		Last Modified: Thu, 03 Aug 2023 02:53:09 GMT  
		Size: 16.2 MB (16177045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fdbcba4b60e13428e996857b320b2f6c63e807e5a913ad4ec5d47030d42cfeb`  
		Last Modified: Thu, 03 Aug 2023 02:53:06 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1541c109b80ce27f2bc1c68b6a83cd6685c14be2db0cd37146cd4fcf03bffc3f`  
		Last Modified: Thu, 03 Aug 2023 02:53:06 GMT  
		Size: 5.5 KB (5493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7eca4eaa545696e30985f6b26d25a046747abd3f0b3780eae19334caec9a26`  
		Last Modified: Tue, 10 Oct 2023 20:31:15 GMT  
		Size: 276.1 MB (276063424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370fffbf4def15c27aaf008f7d51419cfbc303c5bfa36097fbe0fc5b24cd99fa`  
		Last Modified: Tue, 10 Oct 2023 20:30:44 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
