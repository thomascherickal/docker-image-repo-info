## `gazebo:gzserver11-bionic`

```console
$ docker pull gazebo@sha256:a6d6a919d9987f8814a6519fc02da4e466d11dca9065987b1dd9d484e68582ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gazebo:gzserver11-bionic` - linux; amd64

```console
$ docker pull gazebo@sha256:76e0cc264d4a00987a9b47e02372b58926ae492660ef86f312d222b8211c2ff4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.8 MB (277755176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4372707d7c20be13ddaf183ea06bfff35cae3c1a6f3d01e65481af5c4ff05711`
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
# Tue, 07 Jun 2022 02:36:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo11=11.11.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 02:36:45 GMT
EXPOSE 11345
# Tue, 07 Jun 2022 02:36:45 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Tue, 07 Jun 2022 02:36:45 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Tue, 07 Jun 2022 02:36:46 GMT
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
	-	`sha256:9410f2a5e783904a1ff7c4aa996e75295638b23a4e1a0c379666300977120e11`  
		Last Modified: Tue, 07 Jun 2022 02:49:51 GMT  
		Size: 235.5 MB (235486489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c4f7d959a5246b057fbe038854077ab13278828fffdacb19b1036cb3e773f7`  
		Last Modified: Tue, 07 Jun 2022 02:49:21 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
