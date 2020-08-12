<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `varnish`

-	[`varnish:6`](#varnish6)
-	[`varnish:6.0`](#varnish60)
-	[`varnish:6.0.6`](#varnish606)
-	[`varnish:6.0.6-1`](#varnish606-1)
-	[`varnish:6.4`](#varnish64)
-	[`varnish:6.4.0`](#varnish640)
-	[`varnish:6.4.0-1`](#varnish640-1)
-	[`varnish:fresh`](#varnishfresh)
-	[`varnish:latest`](#varnishlatest)
-	[`varnish:stable`](#varnishstable)

## `varnish:6`

```console
$ docker pull varnish@sha256:d2756c2e203b7a7234344495da5eac0b1545bf8edd321338954db1cee15dd11d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6` - linux; amd64

```console
$ docker pull varnish@sha256:796047dc0a7834892d2c19778557213ee79b921ed33d701b17e2f5486e19137b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76767230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d43ade62147980441582d1faa915652ae0e59ab6b468e43383f7600a83ff15a`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:23:57 GMT
ENV VARNISH_VERSION=6.4.0-1~buster
# Tue, 04 Aug 2020 23:23:57 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Aug 2020 22:21:51 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A9897320C397E3A60C03E8BF821AD320F71BFF3D; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish64/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Aug 2020 22:21:51 GMT
WORKDIR /etc/varnish
# Wed, 12 Aug 2020 22:21:51 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Wed, 12 Aug 2020 22:21:51 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 12 Aug 2020 22:21:52 GMT
EXPOSE 80 8443
# Wed, 12 Aug 2020 22:21:52 GMT
CMD []
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c137904a1e0e9fad90bdcb8cc1aa3de75751e58327f7f3e551b8204c76fcd24`  
		Last Modified: Wed, 12 Aug 2020 22:22:26 GMT  
		Size: 49.7 MB (49674657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6224d37fa9015c5b8e012e19ff5e49f04dfa0ab58e9d832e30b4625ba8787403`  
		Last Modified: Wed, 12 Aug 2020 22:22:17 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0`

```console
$ docker pull varnish@sha256:935de9d1818e70b08ed977a6fafcd44e18cc18ed3de41d55ea8b93dcc49ee2d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.0` - linux; amd64

```console
$ docker pull varnish@sha256:61ae0ab7b63934b3dd325de8fa5780e32fc19e15717f51a1a87e810724939510
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67186087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ef7f8dcbbef3e9a4f83407406403885b682627a973c6d9e2606997846cc8ff0`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Aug 2020 15:45:49 GMT
ADD file:16a1ddc40c95b14f8d6c79795047776270ee399f36979aaca45978a67bfee134 in / 
# Tue, 04 Aug 2020 15:45:49 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:23:15 GMT
ENV VARNISH_VERSION=6.0.6-1~stretch
# Tue, 04 Aug 2020 23:23:15 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Aug 2020 22:21:24 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ stretch main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Aug 2020 22:21:24 GMT
WORKDIR /etc/varnish
# Wed, 12 Aug 2020 22:21:24 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Wed, 12 Aug 2020 22:21:24 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 12 Aug 2020 22:21:25 GMT
EXPOSE 80 8443
# Wed, 12 Aug 2020 22:21:25 GMT
CMD []
```

-	Layers:
	-	`sha256:75cb2ebf3b3cb9c601a22edc7d9a120749da33999b30fba22b6cf2b90ee92823`  
		Last Modified: Tue, 04 Aug 2020 15:52:18 GMT  
		Size: 22.5 MB (22522276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfdd05305bbdf69a92affbda813d855afdab2bd9aca8de65211b74046880bf4`  
		Last Modified: Wed, 12 Aug 2020 22:22:11 GMT  
		Size: 44.7 MB (44663349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f664963f8274d4f35cba5f19aaa74767571a748bb614c318f7006037c4cdf5f`  
		Last Modified: Wed, 12 Aug 2020 22:22:02 GMT  
		Size: 462.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0.6`

```console
$ docker pull varnish@sha256:935de9d1818e70b08ed977a6fafcd44e18cc18ed3de41d55ea8b93dcc49ee2d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.0.6` - linux; amd64

```console
$ docker pull varnish@sha256:61ae0ab7b63934b3dd325de8fa5780e32fc19e15717f51a1a87e810724939510
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67186087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ef7f8dcbbef3e9a4f83407406403885b682627a973c6d9e2606997846cc8ff0`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Aug 2020 15:45:49 GMT
ADD file:16a1ddc40c95b14f8d6c79795047776270ee399f36979aaca45978a67bfee134 in / 
# Tue, 04 Aug 2020 15:45:49 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:23:15 GMT
ENV VARNISH_VERSION=6.0.6-1~stretch
# Tue, 04 Aug 2020 23:23:15 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Aug 2020 22:21:24 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ stretch main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Aug 2020 22:21:24 GMT
WORKDIR /etc/varnish
# Wed, 12 Aug 2020 22:21:24 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Wed, 12 Aug 2020 22:21:24 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 12 Aug 2020 22:21:25 GMT
EXPOSE 80 8443
# Wed, 12 Aug 2020 22:21:25 GMT
CMD []
```

-	Layers:
	-	`sha256:75cb2ebf3b3cb9c601a22edc7d9a120749da33999b30fba22b6cf2b90ee92823`  
		Last Modified: Tue, 04 Aug 2020 15:52:18 GMT  
		Size: 22.5 MB (22522276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfdd05305bbdf69a92affbda813d855afdab2bd9aca8de65211b74046880bf4`  
		Last Modified: Wed, 12 Aug 2020 22:22:11 GMT  
		Size: 44.7 MB (44663349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f664963f8274d4f35cba5f19aaa74767571a748bb614c318f7006037c4cdf5f`  
		Last Modified: Wed, 12 Aug 2020 22:22:02 GMT  
		Size: 462.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0.6-1`

```console
$ docker pull varnish@sha256:935de9d1818e70b08ed977a6fafcd44e18cc18ed3de41d55ea8b93dcc49ee2d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.0.6-1` - linux; amd64

```console
$ docker pull varnish@sha256:61ae0ab7b63934b3dd325de8fa5780e32fc19e15717f51a1a87e810724939510
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67186087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ef7f8dcbbef3e9a4f83407406403885b682627a973c6d9e2606997846cc8ff0`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Aug 2020 15:45:49 GMT
ADD file:16a1ddc40c95b14f8d6c79795047776270ee399f36979aaca45978a67bfee134 in / 
# Tue, 04 Aug 2020 15:45:49 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:23:15 GMT
ENV VARNISH_VERSION=6.0.6-1~stretch
# Tue, 04 Aug 2020 23:23:15 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Aug 2020 22:21:24 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ stretch main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Aug 2020 22:21:24 GMT
WORKDIR /etc/varnish
# Wed, 12 Aug 2020 22:21:24 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Wed, 12 Aug 2020 22:21:24 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 12 Aug 2020 22:21:25 GMT
EXPOSE 80 8443
# Wed, 12 Aug 2020 22:21:25 GMT
CMD []
```

-	Layers:
	-	`sha256:75cb2ebf3b3cb9c601a22edc7d9a120749da33999b30fba22b6cf2b90ee92823`  
		Last Modified: Tue, 04 Aug 2020 15:52:18 GMT  
		Size: 22.5 MB (22522276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfdd05305bbdf69a92affbda813d855afdab2bd9aca8de65211b74046880bf4`  
		Last Modified: Wed, 12 Aug 2020 22:22:11 GMT  
		Size: 44.7 MB (44663349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f664963f8274d4f35cba5f19aaa74767571a748bb614c318f7006037c4cdf5f`  
		Last Modified: Wed, 12 Aug 2020 22:22:02 GMT  
		Size: 462.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.4`

```console
$ docker pull varnish@sha256:d2756c2e203b7a7234344495da5eac0b1545bf8edd321338954db1cee15dd11d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.4` - linux; amd64

```console
$ docker pull varnish@sha256:796047dc0a7834892d2c19778557213ee79b921ed33d701b17e2f5486e19137b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76767230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d43ade62147980441582d1faa915652ae0e59ab6b468e43383f7600a83ff15a`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:23:57 GMT
ENV VARNISH_VERSION=6.4.0-1~buster
# Tue, 04 Aug 2020 23:23:57 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Aug 2020 22:21:51 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A9897320C397E3A60C03E8BF821AD320F71BFF3D; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish64/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Aug 2020 22:21:51 GMT
WORKDIR /etc/varnish
# Wed, 12 Aug 2020 22:21:51 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Wed, 12 Aug 2020 22:21:51 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 12 Aug 2020 22:21:52 GMT
EXPOSE 80 8443
# Wed, 12 Aug 2020 22:21:52 GMT
CMD []
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c137904a1e0e9fad90bdcb8cc1aa3de75751e58327f7f3e551b8204c76fcd24`  
		Last Modified: Wed, 12 Aug 2020 22:22:26 GMT  
		Size: 49.7 MB (49674657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6224d37fa9015c5b8e012e19ff5e49f04dfa0ab58e9d832e30b4625ba8787403`  
		Last Modified: Wed, 12 Aug 2020 22:22:17 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.4.0`

```console
$ docker pull varnish@sha256:d2756c2e203b7a7234344495da5eac0b1545bf8edd321338954db1cee15dd11d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.4.0` - linux; amd64

```console
$ docker pull varnish@sha256:796047dc0a7834892d2c19778557213ee79b921ed33d701b17e2f5486e19137b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76767230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d43ade62147980441582d1faa915652ae0e59ab6b468e43383f7600a83ff15a`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:23:57 GMT
ENV VARNISH_VERSION=6.4.0-1~buster
# Tue, 04 Aug 2020 23:23:57 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Aug 2020 22:21:51 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A9897320C397E3A60C03E8BF821AD320F71BFF3D; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish64/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Aug 2020 22:21:51 GMT
WORKDIR /etc/varnish
# Wed, 12 Aug 2020 22:21:51 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Wed, 12 Aug 2020 22:21:51 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 12 Aug 2020 22:21:52 GMT
EXPOSE 80 8443
# Wed, 12 Aug 2020 22:21:52 GMT
CMD []
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c137904a1e0e9fad90bdcb8cc1aa3de75751e58327f7f3e551b8204c76fcd24`  
		Last Modified: Wed, 12 Aug 2020 22:22:26 GMT  
		Size: 49.7 MB (49674657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6224d37fa9015c5b8e012e19ff5e49f04dfa0ab58e9d832e30b4625ba8787403`  
		Last Modified: Wed, 12 Aug 2020 22:22:17 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.4.0-1`

```console
$ docker pull varnish@sha256:d2756c2e203b7a7234344495da5eac0b1545bf8edd321338954db1cee15dd11d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.4.0-1` - linux; amd64

```console
$ docker pull varnish@sha256:796047dc0a7834892d2c19778557213ee79b921ed33d701b17e2f5486e19137b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76767230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d43ade62147980441582d1faa915652ae0e59ab6b468e43383f7600a83ff15a`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:23:57 GMT
ENV VARNISH_VERSION=6.4.0-1~buster
# Tue, 04 Aug 2020 23:23:57 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Aug 2020 22:21:51 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A9897320C397E3A60C03E8BF821AD320F71BFF3D; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish64/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Aug 2020 22:21:51 GMT
WORKDIR /etc/varnish
# Wed, 12 Aug 2020 22:21:51 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Wed, 12 Aug 2020 22:21:51 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 12 Aug 2020 22:21:52 GMT
EXPOSE 80 8443
# Wed, 12 Aug 2020 22:21:52 GMT
CMD []
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c137904a1e0e9fad90bdcb8cc1aa3de75751e58327f7f3e551b8204c76fcd24`  
		Last Modified: Wed, 12 Aug 2020 22:22:26 GMT  
		Size: 49.7 MB (49674657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6224d37fa9015c5b8e012e19ff5e49f04dfa0ab58e9d832e30b4625ba8787403`  
		Last Modified: Wed, 12 Aug 2020 22:22:17 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:fresh`

```console
$ docker pull varnish@sha256:d2756c2e203b7a7234344495da5eac0b1545bf8edd321338954db1cee15dd11d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:fresh` - linux; amd64

```console
$ docker pull varnish@sha256:796047dc0a7834892d2c19778557213ee79b921ed33d701b17e2f5486e19137b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76767230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d43ade62147980441582d1faa915652ae0e59ab6b468e43383f7600a83ff15a`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:23:57 GMT
ENV VARNISH_VERSION=6.4.0-1~buster
# Tue, 04 Aug 2020 23:23:57 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Aug 2020 22:21:51 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A9897320C397E3A60C03E8BF821AD320F71BFF3D; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish64/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Aug 2020 22:21:51 GMT
WORKDIR /etc/varnish
# Wed, 12 Aug 2020 22:21:51 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Wed, 12 Aug 2020 22:21:51 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 12 Aug 2020 22:21:52 GMT
EXPOSE 80 8443
# Wed, 12 Aug 2020 22:21:52 GMT
CMD []
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c137904a1e0e9fad90bdcb8cc1aa3de75751e58327f7f3e551b8204c76fcd24`  
		Last Modified: Wed, 12 Aug 2020 22:22:26 GMT  
		Size: 49.7 MB (49674657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6224d37fa9015c5b8e012e19ff5e49f04dfa0ab58e9d832e30b4625ba8787403`  
		Last Modified: Wed, 12 Aug 2020 22:22:17 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:latest`

```console
$ docker pull varnish@sha256:d2756c2e203b7a7234344495da5eac0b1545bf8edd321338954db1cee15dd11d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:latest` - linux; amd64

```console
$ docker pull varnish@sha256:796047dc0a7834892d2c19778557213ee79b921ed33d701b17e2f5486e19137b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76767230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d43ade62147980441582d1faa915652ae0e59ab6b468e43383f7600a83ff15a`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:23:57 GMT
ENV VARNISH_VERSION=6.4.0-1~buster
# Tue, 04 Aug 2020 23:23:57 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Aug 2020 22:21:51 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A9897320C397E3A60C03E8BF821AD320F71BFF3D; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish64/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Aug 2020 22:21:51 GMT
WORKDIR /etc/varnish
# Wed, 12 Aug 2020 22:21:51 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Wed, 12 Aug 2020 22:21:51 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 12 Aug 2020 22:21:52 GMT
EXPOSE 80 8443
# Wed, 12 Aug 2020 22:21:52 GMT
CMD []
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c137904a1e0e9fad90bdcb8cc1aa3de75751e58327f7f3e551b8204c76fcd24`  
		Last Modified: Wed, 12 Aug 2020 22:22:26 GMT  
		Size: 49.7 MB (49674657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6224d37fa9015c5b8e012e19ff5e49f04dfa0ab58e9d832e30b4625ba8787403`  
		Last Modified: Wed, 12 Aug 2020 22:22:17 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:stable`

```console
$ docker pull varnish@sha256:935de9d1818e70b08ed977a6fafcd44e18cc18ed3de41d55ea8b93dcc49ee2d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:stable` - linux; amd64

```console
$ docker pull varnish@sha256:61ae0ab7b63934b3dd325de8fa5780e32fc19e15717f51a1a87e810724939510
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67186087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ef7f8dcbbef3e9a4f83407406403885b682627a973c6d9e2606997846cc8ff0`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Aug 2020 15:45:49 GMT
ADD file:16a1ddc40c95b14f8d6c79795047776270ee399f36979aaca45978a67bfee134 in / 
# Tue, 04 Aug 2020 15:45:49 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:23:15 GMT
ENV VARNISH_VERSION=6.0.6-1~stretch
# Tue, 04 Aug 2020 23:23:15 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Aug 2020 22:21:24 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ stretch main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Aug 2020 22:21:24 GMT
WORKDIR /etc/varnish
# Wed, 12 Aug 2020 22:21:24 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Wed, 12 Aug 2020 22:21:24 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 12 Aug 2020 22:21:25 GMT
EXPOSE 80 8443
# Wed, 12 Aug 2020 22:21:25 GMT
CMD []
```

-	Layers:
	-	`sha256:75cb2ebf3b3cb9c601a22edc7d9a120749da33999b30fba22b6cf2b90ee92823`  
		Last Modified: Tue, 04 Aug 2020 15:52:18 GMT  
		Size: 22.5 MB (22522276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfdd05305bbdf69a92affbda813d855afdab2bd9aca8de65211b74046880bf4`  
		Last Modified: Wed, 12 Aug 2020 22:22:11 GMT  
		Size: 44.7 MB (44663349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f664963f8274d4f35cba5f19aaa74767571a748bb614c318f7006037c4cdf5f`  
		Last Modified: Wed, 12 Aug 2020 22:22:02 GMT  
		Size: 462.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
