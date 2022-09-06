## `gazebo:gzserver11-bionic`

```console
$ docker pull gazebo@sha256:0d43b11fea5747a26075e0f2ad9fbfdf8b287141504726d969e3a3a3b1af2ae8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gazebo:gzserver11-bionic` - linux; amd64

```console
$ docker pull gazebo@sha256:487f69654cb05d7f667f24c05dfbbb86d702ae19d44e02551d058c56530867e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.8 MB (277802128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6075f291c6b8be3d3e0fd7118eb243d2634b2fa25dc6a3546e27ffc6eb1beaec`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Tue, 06 Sep 2022 19:38:36 GMT
ADD file:8733c7e8faf03d53cb2143ff6ac405362944cfa07422fccd21a3066cc2f42c83 in / 
# Tue, 06 Sep 2022 19:38:37 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 20:08:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 20:08:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 20:08:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Tue, 06 Sep 2022 20:08:14 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Tue, 06 Sep 2022 20:13:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo11=11.11.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 20:13:47 GMT
EXPOSE 11345
# Tue, 06 Sep 2022 20:13:47 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Tue, 06 Sep 2022 20:13:48 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Tue, 06 Sep 2022 20:13:48 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:726b8a513d66e3585eb57389171d97fcd348e4914a415891e1da135b85ffa6c3`  
		Last Modified: Fri, 02 Sep 2022 15:41:13 GMT  
		Size: 26.7 MB (26710833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4768d9bcc163805ab5ecfee0d555df97a3b8eaadc5b4bf8e8b458c12e089102a`  
		Last Modified: Tue, 06 Sep 2022 20:16:26 GMT  
		Size: 831.0 KB (830982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d4d0f23e3d912c53609ab1be508ea52480495f1e93e47c5e2b107c4969b20f`  
		Last Modified: Tue, 06 Sep 2022 20:16:26 GMT  
		Size: 14.7 MB (14709179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf438ef6aac76bc018f4485e7292597740d514f8946170fe8b20ae459c909228`  
		Last Modified: Tue, 06 Sep 2022 20:16:24 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94106123bc7e51b0b61ac37d458ee8f95ec1b09e442f9c245cab9638803c3a5e`  
		Last Modified: Tue, 06 Sep 2022 20:16:24 GMT  
		Size: 5.5 KB (5460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffbb9399606d3a91bc04f0bc0605e3938ff58ba848caeead21cfe19100cc63e`  
		Last Modified: Tue, 06 Sep 2022 20:18:10 GMT  
		Size: 235.5 MB (235544046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b81ef8e906dd52baf683359b621caee90d12359b0c6410bdef0de7b04885d62`  
		Last Modified: Tue, 06 Sep 2022 20:17:41 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
