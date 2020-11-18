## `buildpack-deps:oldoldstable-curl`

```console
$ docker pull buildpack-deps@sha256:3fc3400256f1e951e08bd68ac43f1f7b5d02668c494c59ef55d50398b8741d1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `buildpack-deps:oldoldstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:f8169278ee09a58369d749f09bc8b257c6bcb7cb6f70cbde7201f573b163d4d5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71934416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d13eea65991574176e6c32f90c1eea11daa4ea2a8b06f9c36d19df923eac2143`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:33 GMT
ADD file:a6871f73455488933c1b46ec3a892d3db537f631c01e75573369c7c45b41d017 in / 
# Tue, 17 Nov 2020 20:21:33 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 00:34:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:34:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:dbcd895dc67d5ce0b25d47678d747226ed725a22e31901fc021fd23879b1ccfe`  
		Last Modified: Tue, 17 Nov 2020 20:27:44 GMT  
		Size: 54.4 MB (54388442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74c5e680cac4523e977d5f2e4e08afec0feb025fba9c24c0c340d4b5ec0d414`  
		Last Modified: Wed, 18 Nov 2020 00:51:29 GMT  
		Size: 17.5 MB (17545974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:adf3b0f4a487ad5fea1181ca5995656ae17c0faa86f2b2a25980d2db2686f617
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69620011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:911a60057036ac0988f989ddb842b8378c6578599781a7def4af5d9c1dfc735d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:09 GMT
ADD file:06d0d96a3590043e004bbd651614b8c1b4b048df6ce8706542c12613e2ef83f3 in / 
# Tue, 17 Nov 2020 20:21:10 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:47:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:47:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2950e78c0ac6ca79b0455caabb98b5d25fa715881ced046fe07f25029b96bd01`  
		Last Modified: Tue, 17 Nov 2020 20:30:58 GMT  
		Size: 52.6 MB (52582709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d215fc87b1798e34927476d1004914e87fa45af53379310422e62443ed2654`  
		Last Modified: Tue, 17 Nov 2020 22:10:02 GMT  
		Size: 17.0 MB (17037302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:79ae1bda1a22d52a8061221d189f9085d9e899444f5a5c5375e0d01ee11d2df0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (67028641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4147bbc14a72d7310e55211aed16dfa0df6a006edb0afa5f0fe4381e20a0c6a2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:34 GMT
ADD file:b2545152b2d5298539a3587be3ec1f7ecfececebb4ee80eaff97f66143feac5e in / 
# Tue, 17 Nov 2020 20:21:35 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:46:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:46:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d4af4a46f2c554db32c2423a35e7d1fd96ec1a41633404963392957596e60a5b`  
		Last Modified: Tue, 17 Nov 2020 20:32:10 GMT  
		Size: 50.3 MB (50305387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc5e67e7f7b7f724bbb49fbc0795a7c5d76ac00b944870eb1d2ea3a69994caa`  
		Last Modified: Tue, 17 Nov 2020 22:08:52 GMT  
		Size: 16.7 MB (16723254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:5553bcc1c77a5c1b77207790e17323d6c0be000a3f3e832943b3f5ab0b5173d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.5 MB (74464725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa4b35e65dcf4699a6bdecec9aaa3c094b3d82c184be2bce1551ea2e619a7fab`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:20:16 GMT
ADD file:843de10973ffdcb28448f75b968c0f3f47adc33e3bb0fa5adf1c488c8fbbf5f1 in / 
# Tue, 17 Nov 2020 20:20:16 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:09:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:09:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b79b7651073e6b6c71d7e4168850a7ded5ca4e7d948a7035975a0e83ad6703c6`  
		Last Modified: Tue, 17 Nov 2020 20:27:07 GMT  
		Size: 54.6 MB (54608823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c14b2d754487de7f15aff3e85e50a59c7af0d8f0fcd3ce1c40e8ec436e5fb2d`  
		Last Modified: Tue, 17 Nov 2020 21:25:19 GMT  
		Size: 19.9 MB (19855902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
