## `gazebo:latest`

```console
$ docker pull gazebo@sha256:c2e9885ad6b9e640b218e82e35dfa42f19060eca4a5956368c97173ef4eefc5e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gazebo:latest` - linux; amd64

```console
$ docker pull gazebo@sha256:4cc52c60a14194a4f81ead7972e17c3265973e649c32d7391ef2008dc81caa0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **615.7 MB (615679094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68d4b191f02c2c3d23b0dd340c812e2046d24cb0341b567a665334b2c754cdd7`
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
# Tue, 10 Oct 2023 20:30:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     libgazebo11-dev=11.14.0-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:bc9308be39cad1a60d43807fbc2fa8074b2e7c91804773ca4dd1f2c8edebcac9`  
		Last Modified: Tue, 10 Oct 2023 20:32:10 GMT  
		Size: 293.7 MB (293652210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
