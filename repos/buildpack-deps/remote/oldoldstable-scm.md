## `buildpack-deps:oldoldstable-scm`

```console
$ docker pull buildpack-deps@sha256:485b03b033e2741e0377ebb448dbc172ed36632d062dc9ddd68d7e18a754d687
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `buildpack-deps:oldoldstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:694e67b054793477b5cb90e7e9f504d18616719471c7fa9acbd0e464ef762680
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.3 MB (115269105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a6e780ddb8590e6e297a5f26adf79418d021b32ae6c3da0d6922f4b1fb0077d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 00:24:00 GMT
ADD file:ca64ef47722e4bf4beeab729a34cd854fe7293a0a2a0a2a92e6f1347c071dfe9 in / 
# Thu, 10 Sep 2020 00:24:01 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 01:03:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 01:03:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 01:05:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:290431e500161a90ac38ac8631791acb27e14a913613b60b3df58f839168df40`  
		Last Modified: Thu, 10 Sep 2020 00:34:21 GMT  
		Size: 54.4 MB (54389019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcaf1dd00a337044e2c0421947b13d7390883ef55a08ff9ea58d13ce59784328`  
		Last Modified: Thu, 10 Sep 2020 01:16:59 GMT  
		Size: 17.5 MB (17545982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478d2f36706aba42a38a1d269f4e5f9e733730c04955e96a04d508b1cd9d589f`  
		Last Modified: Thu, 10 Sep 2020 01:17:17 GMT  
		Size: 43.3 MB (43334104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:5661f9fcc212db92ccd44eeb7f5238fd0bb4e860bffb5f8e3bcd5a2a85335df7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.8 MB (110776885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:407674c93506eaf522e0df62a2e3bab72fc66d7927f3acc8b5f53b0d977d15aa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:54:15 GMT
ADD file:b5770ada526014c416df31779f0c640c62a5e53e8e018a6201d507999ac34e18 in / 
# Wed, 09 Sep 2020 23:54:19 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:37:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:37:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 00:38:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:82ebff95f0e21d655344637482b367c7ea0db41b80cbc667bd980d2141287029`  
		Last Modified: Thu, 10 Sep 2020 00:03:15 GMT  
		Size: 52.6 MB (52583713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f40e46cda9c751ff385c796d48a3c39740220c3885866739fe62640f9437afa`  
		Last Modified: Thu, 10 Sep 2020 00:55:04 GMT  
		Size: 17.0 MB (17037321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9bd6814b5011e45af4aaee011465ebcf614eef4d29dab5a87d8a3fed3655f0`  
		Last Modified: Thu, 10 Sep 2020 00:55:28 GMT  
		Size: 41.2 MB (41155851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:dc6e4ea0322331efa6c1378d8b2183b3c978e5a0237fb117e8f2ed3f6c1616b3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106808152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1749970c4c9b178ba7834e3ae81bb396b99426465aff78bff44293737f83759`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:57:16 GMT
ADD file:1b4bf8acda0b906341b6a17ca6eccc23744ba196c78c5bc59c3e26d0b2ebe596 in / 
# Tue, 04 Aug 2020 04:57:18 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:00:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 08:00:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 08:02:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7c58b357cec76336de1011b56cc2999a53017c6a4b3cf93f2b8362b7a055c544`  
		Last Modified: Tue, 04 Aug 2020 05:05:41 GMT  
		Size: 50.3 MB (50305564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64410aa4323d878bbe3be9802befcd90ffd5681624e0e325a80f25a038fa6cc`  
		Last Modified: Tue, 04 Aug 2020 08:27:38 GMT  
		Size: 16.7 MB (16723645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ff21f785d375d1e97b8335d239d9cfbfffe0b0706afae0679ffd7f6c202157`  
		Last Modified: Tue, 04 Aug 2020 08:28:04 GMT  
		Size: 39.8 MB (39778943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:2d057f5e909c9c72f6e4738b18cb6b3190229045d2a9a8e140656f5499f1a820
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118456014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ff8680d043d4076e1d5e86f3506aedabac33f30e9d8cfa4727f5e9c9e84c32a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:49 GMT
ADD file:85c105a2f2f0c7bff57c73bff9ecdb5ae2cb04074a0129fc1a82d4da85b95ec0 in / 
# Tue, 04 Aug 2020 03:37:49 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:11:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 08:11:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 08:14:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:49a2d30c774cb18fa05d4cb6f730f97f4965b1162debd13f35bf1733bb737735`  
		Last Modified: Tue, 04 Aug 2020 03:42:50 GMT  
		Size: 54.6 MB (54609569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb76cc7bc12f41ea0e34f0355c0a2d2c5689a14b42947760e1caf7b92ff80dc`  
		Last Modified: Tue, 04 Aug 2020 08:27:50 GMT  
		Size: 19.9 MB (19855978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d975d21db51982cf56382647589c692e4b2d94ca28355895c5bd8514ad38b0`  
		Last Modified: Tue, 04 Aug 2020 08:28:07 GMT  
		Size: 44.0 MB (43990467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
