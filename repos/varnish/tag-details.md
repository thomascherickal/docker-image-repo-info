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
$ docker pull varnish@sha256:c7fbf7c5fa5c5b1ee4b512c0237740136d86551f04c54376c80e7436a47ae994
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6` - linux; amd64

```console
$ docker pull varnish@sha256:33901580d26fb83093fe4f5d3bf9dc949c6041054e1148cfae3e8a287af760b1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76767889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b6d153e995c84a2649a50836407ea9ea25a4839102e0755010109b045ce2a9e`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 26 Feb 2020 00:37:39 GMT
ADD file:e5a364615e0f6961626089c7d658adbf8c8d95b3ae95a390a8bb33875317d434 in / 
# Wed, 26 Feb 2020 00:37:39 GMT
CMD ["bash"]
# Wed, 25 Mar 2020 21:32:36 GMT
ENV VARNISH_VERSION=6.4.0-1~buster
# Wed, 25 Mar 2020 21:32:37 GMT
ENV VARNISH_SIZE=100M
# Wed, 25 Mar 2020 21:32:57 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A9897320C397E3A60C03E8BF821AD320F71BFF3D; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish64/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Mar 2020 21:32:57 GMT
WORKDIR /etc/varnish
# Wed, 25 Mar 2020 21:32:57 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Wed, 25 Mar 2020 21:32:57 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 25 Mar 2020 21:32:58 GMT
EXPOSE 80 8443
# Wed, 25 Mar 2020 21:32:58 GMT
CMD []
```

-	Layers:
	-	`sha256:68ced04f60ab5c7a5f1d0b0b4e7572c5a4c8cce44866513d30d9df1a15277d6b`  
		Last Modified: Wed, 26 Feb 2020 00:44:23 GMT  
		Size: 27.1 MB (27091819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9baf6d7f5902865b7612b931e32e7fe4d6c4181522242b5ae5c6a3ef70d6b9`  
		Last Modified: Wed, 25 Mar 2020 21:33:31 GMT  
		Size: 49.7 MB (49675617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8f0f9612b31b862a504cee5b804f160110ba8780faf749bdc2825da5f00123`  
		Last Modified: Wed, 25 Mar 2020 21:33:22 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0`

```console
$ docker pull varnish@sha256:c6e4b319a3d57b427dd6c2e362b262da172c49228e7af0693f37a1e15c04efd0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.0` - linux; amd64

```console
$ docker pull varnish@sha256:acf859b396f9c8643d1a7ec838f034cc2cddaac8ab629996f9451d864a231917
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67208285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e64007059f2bf0a704900b4172bd3c00b82ac9e22aed9b55928a17b21e9cfdf`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 26 Feb 2020 00:41:38 GMT
ADD file:1256c62f77a54c982fdb2790d682049b2ad64c8466466e846f3d33ad1ed4035d in / 
# Wed, 26 Feb 2020 00:41:38 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 20:13:14 GMT
ENV VARNISH_VERSION=6.0.6-1~stretch
# Wed, 25 Mar 2020 21:31:55 GMT
ENV VARNISH_SIZE=100M
# Wed, 25 Mar 2020 21:32:31 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ stretch main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Mar 2020 21:32:31 GMT
WORKDIR /etc/varnish
# Wed, 25 Mar 2020 21:32:32 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Wed, 25 Mar 2020 21:32:32 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 25 Mar 2020 21:32:32 GMT
EXPOSE 80 8443
# Wed, 25 Mar 2020 21:32:32 GMT
CMD []
```

-	Layers:
	-	`sha256:6d28e14ab8c85bf8a4331de0667c27d19ef4092b12531eec0334b5c2a1012668`  
		Last Modified: Wed, 26 Feb 2020 00:47:21 GMT  
		Size: 22.5 MB (22513365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a559f845f03a758956a7405ece4724da82a6e83566f70bb634b81b3d049232a9`  
		Last Modified: Wed, 25 Mar 2020 21:33:17 GMT  
		Size: 44.7 MB (44694459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148a380b311faddf915d592cd6befeda285bee881c1cee42c2a124891b627239`  
		Last Modified: Wed, 25 Mar 2020 21:33:09 GMT  
		Size: 461.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0.6`

```console
$ docker pull varnish@sha256:c6e4b319a3d57b427dd6c2e362b262da172c49228e7af0693f37a1e15c04efd0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.0.6` - linux; amd64

```console
$ docker pull varnish@sha256:acf859b396f9c8643d1a7ec838f034cc2cddaac8ab629996f9451d864a231917
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67208285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e64007059f2bf0a704900b4172bd3c00b82ac9e22aed9b55928a17b21e9cfdf`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 26 Feb 2020 00:41:38 GMT
ADD file:1256c62f77a54c982fdb2790d682049b2ad64c8466466e846f3d33ad1ed4035d in / 
# Wed, 26 Feb 2020 00:41:38 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 20:13:14 GMT
ENV VARNISH_VERSION=6.0.6-1~stretch
# Wed, 25 Mar 2020 21:31:55 GMT
ENV VARNISH_SIZE=100M
# Wed, 25 Mar 2020 21:32:31 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ stretch main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Mar 2020 21:32:31 GMT
WORKDIR /etc/varnish
# Wed, 25 Mar 2020 21:32:32 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Wed, 25 Mar 2020 21:32:32 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 25 Mar 2020 21:32:32 GMT
EXPOSE 80 8443
# Wed, 25 Mar 2020 21:32:32 GMT
CMD []
```

-	Layers:
	-	`sha256:6d28e14ab8c85bf8a4331de0667c27d19ef4092b12531eec0334b5c2a1012668`  
		Last Modified: Wed, 26 Feb 2020 00:47:21 GMT  
		Size: 22.5 MB (22513365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a559f845f03a758956a7405ece4724da82a6e83566f70bb634b81b3d049232a9`  
		Last Modified: Wed, 25 Mar 2020 21:33:17 GMT  
		Size: 44.7 MB (44694459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148a380b311faddf915d592cd6befeda285bee881c1cee42c2a124891b627239`  
		Last Modified: Wed, 25 Mar 2020 21:33:09 GMT  
		Size: 461.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0.6-1`

```console
$ docker pull varnish@sha256:c6e4b319a3d57b427dd6c2e362b262da172c49228e7af0693f37a1e15c04efd0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.0.6-1` - linux; amd64

```console
$ docker pull varnish@sha256:acf859b396f9c8643d1a7ec838f034cc2cddaac8ab629996f9451d864a231917
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67208285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e64007059f2bf0a704900b4172bd3c00b82ac9e22aed9b55928a17b21e9cfdf`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 26 Feb 2020 00:41:38 GMT
ADD file:1256c62f77a54c982fdb2790d682049b2ad64c8466466e846f3d33ad1ed4035d in / 
# Wed, 26 Feb 2020 00:41:38 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 20:13:14 GMT
ENV VARNISH_VERSION=6.0.6-1~stretch
# Wed, 25 Mar 2020 21:31:55 GMT
ENV VARNISH_SIZE=100M
# Wed, 25 Mar 2020 21:32:31 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ stretch main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Mar 2020 21:32:31 GMT
WORKDIR /etc/varnish
# Wed, 25 Mar 2020 21:32:32 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Wed, 25 Mar 2020 21:32:32 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 25 Mar 2020 21:32:32 GMT
EXPOSE 80 8443
# Wed, 25 Mar 2020 21:32:32 GMT
CMD []
```

-	Layers:
	-	`sha256:6d28e14ab8c85bf8a4331de0667c27d19ef4092b12531eec0334b5c2a1012668`  
		Last Modified: Wed, 26 Feb 2020 00:47:21 GMT  
		Size: 22.5 MB (22513365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a559f845f03a758956a7405ece4724da82a6e83566f70bb634b81b3d049232a9`  
		Last Modified: Wed, 25 Mar 2020 21:33:17 GMT  
		Size: 44.7 MB (44694459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148a380b311faddf915d592cd6befeda285bee881c1cee42c2a124891b627239`  
		Last Modified: Wed, 25 Mar 2020 21:33:09 GMT  
		Size: 461.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.4`

```console
$ docker pull varnish@sha256:c7fbf7c5fa5c5b1ee4b512c0237740136d86551f04c54376c80e7436a47ae994
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.4` - linux; amd64

```console
$ docker pull varnish@sha256:33901580d26fb83093fe4f5d3bf9dc949c6041054e1148cfae3e8a287af760b1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76767889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b6d153e995c84a2649a50836407ea9ea25a4839102e0755010109b045ce2a9e`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 26 Feb 2020 00:37:39 GMT
ADD file:e5a364615e0f6961626089c7d658adbf8c8d95b3ae95a390a8bb33875317d434 in / 
# Wed, 26 Feb 2020 00:37:39 GMT
CMD ["bash"]
# Wed, 25 Mar 2020 21:32:36 GMT
ENV VARNISH_VERSION=6.4.0-1~buster
# Wed, 25 Mar 2020 21:32:37 GMT
ENV VARNISH_SIZE=100M
# Wed, 25 Mar 2020 21:32:57 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A9897320C397E3A60C03E8BF821AD320F71BFF3D; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish64/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Mar 2020 21:32:57 GMT
WORKDIR /etc/varnish
# Wed, 25 Mar 2020 21:32:57 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Wed, 25 Mar 2020 21:32:57 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 25 Mar 2020 21:32:58 GMT
EXPOSE 80 8443
# Wed, 25 Mar 2020 21:32:58 GMT
CMD []
```

-	Layers:
	-	`sha256:68ced04f60ab5c7a5f1d0b0b4e7572c5a4c8cce44866513d30d9df1a15277d6b`  
		Last Modified: Wed, 26 Feb 2020 00:44:23 GMT  
		Size: 27.1 MB (27091819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9baf6d7f5902865b7612b931e32e7fe4d6c4181522242b5ae5c6a3ef70d6b9`  
		Last Modified: Wed, 25 Mar 2020 21:33:31 GMT  
		Size: 49.7 MB (49675617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8f0f9612b31b862a504cee5b804f160110ba8780faf749bdc2825da5f00123`  
		Last Modified: Wed, 25 Mar 2020 21:33:22 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.4.0`

```console
$ docker pull varnish@sha256:c7fbf7c5fa5c5b1ee4b512c0237740136d86551f04c54376c80e7436a47ae994
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.4.0` - linux; amd64

```console
$ docker pull varnish@sha256:33901580d26fb83093fe4f5d3bf9dc949c6041054e1148cfae3e8a287af760b1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76767889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b6d153e995c84a2649a50836407ea9ea25a4839102e0755010109b045ce2a9e`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 26 Feb 2020 00:37:39 GMT
ADD file:e5a364615e0f6961626089c7d658adbf8c8d95b3ae95a390a8bb33875317d434 in / 
# Wed, 26 Feb 2020 00:37:39 GMT
CMD ["bash"]
# Wed, 25 Mar 2020 21:32:36 GMT
ENV VARNISH_VERSION=6.4.0-1~buster
# Wed, 25 Mar 2020 21:32:37 GMT
ENV VARNISH_SIZE=100M
# Wed, 25 Mar 2020 21:32:57 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A9897320C397E3A60C03E8BF821AD320F71BFF3D; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish64/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Mar 2020 21:32:57 GMT
WORKDIR /etc/varnish
# Wed, 25 Mar 2020 21:32:57 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Wed, 25 Mar 2020 21:32:57 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 25 Mar 2020 21:32:58 GMT
EXPOSE 80 8443
# Wed, 25 Mar 2020 21:32:58 GMT
CMD []
```

-	Layers:
	-	`sha256:68ced04f60ab5c7a5f1d0b0b4e7572c5a4c8cce44866513d30d9df1a15277d6b`  
		Last Modified: Wed, 26 Feb 2020 00:44:23 GMT  
		Size: 27.1 MB (27091819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9baf6d7f5902865b7612b931e32e7fe4d6c4181522242b5ae5c6a3ef70d6b9`  
		Last Modified: Wed, 25 Mar 2020 21:33:31 GMT  
		Size: 49.7 MB (49675617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8f0f9612b31b862a504cee5b804f160110ba8780faf749bdc2825da5f00123`  
		Last Modified: Wed, 25 Mar 2020 21:33:22 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.4.0-1`

```console
$ docker pull varnish@sha256:c7fbf7c5fa5c5b1ee4b512c0237740136d86551f04c54376c80e7436a47ae994
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.4.0-1` - linux; amd64

```console
$ docker pull varnish@sha256:33901580d26fb83093fe4f5d3bf9dc949c6041054e1148cfae3e8a287af760b1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76767889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b6d153e995c84a2649a50836407ea9ea25a4839102e0755010109b045ce2a9e`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 26 Feb 2020 00:37:39 GMT
ADD file:e5a364615e0f6961626089c7d658adbf8c8d95b3ae95a390a8bb33875317d434 in / 
# Wed, 26 Feb 2020 00:37:39 GMT
CMD ["bash"]
# Wed, 25 Mar 2020 21:32:36 GMT
ENV VARNISH_VERSION=6.4.0-1~buster
# Wed, 25 Mar 2020 21:32:37 GMT
ENV VARNISH_SIZE=100M
# Wed, 25 Mar 2020 21:32:57 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A9897320C397E3A60C03E8BF821AD320F71BFF3D; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish64/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Mar 2020 21:32:57 GMT
WORKDIR /etc/varnish
# Wed, 25 Mar 2020 21:32:57 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Wed, 25 Mar 2020 21:32:57 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 25 Mar 2020 21:32:58 GMT
EXPOSE 80 8443
# Wed, 25 Mar 2020 21:32:58 GMT
CMD []
```

-	Layers:
	-	`sha256:68ced04f60ab5c7a5f1d0b0b4e7572c5a4c8cce44866513d30d9df1a15277d6b`  
		Last Modified: Wed, 26 Feb 2020 00:44:23 GMT  
		Size: 27.1 MB (27091819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9baf6d7f5902865b7612b931e32e7fe4d6c4181522242b5ae5c6a3ef70d6b9`  
		Last Modified: Wed, 25 Mar 2020 21:33:31 GMT  
		Size: 49.7 MB (49675617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8f0f9612b31b862a504cee5b804f160110ba8780faf749bdc2825da5f00123`  
		Last Modified: Wed, 25 Mar 2020 21:33:22 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:fresh`

```console
$ docker pull varnish@sha256:c7fbf7c5fa5c5b1ee4b512c0237740136d86551f04c54376c80e7436a47ae994
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:fresh` - linux; amd64

```console
$ docker pull varnish@sha256:33901580d26fb83093fe4f5d3bf9dc949c6041054e1148cfae3e8a287af760b1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76767889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b6d153e995c84a2649a50836407ea9ea25a4839102e0755010109b045ce2a9e`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 26 Feb 2020 00:37:39 GMT
ADD file:e5a364615e0f6961626089c7d658adbf8c8d95b3ae95a390a8bb33875317d434 in / 
# Wed, 26 Feb 2020 00:37:39 GMT
CMD ["bash"]
# Wed, 25 Mar 2020 21:32:36 GMT
ENV VARNISH_VERSION=6.4.0-1~buster
# Wed, 25 Mar 2020 21:32:37 GMT
ENV VARNISH_SIZE=100M
# Wed, 25 Mar 2020 21:32:57 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A9897320C397E3A60C03E8BF821AD320F71BFF3D; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish64/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Mar 2020 21:32:57 GMT
WORKDIR /etc/varnish
# Wed, 25 Mar 2020 21:32:57 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Wed, 25 Mar 2020 21:32:57 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 25 Mar 2020 21:32:58 GMT
EXPOSE 80 8443
# Wed, 25 Mar 2020 21:32:58 GMT
CMD []
```

-	Layers:
	-	`sha256:68ced04f60ab5c7a5f1d0b0b4e7572c5a4c8cce44866513d30d9df1a15277d6b`  
		Last Modified: Wed, 26 Feb 2020 00:44:23 GMT  
		Size: 27.1 MB (27091819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9baf6d7f5902865b7612b931e32e7fe4d6c4181522242b5ae5c6a3ef70d6b9`  
		Last Modified: Wed, 25 Mar 2020 21:33:31 GMT  
		Size: 49.7 MB (49675617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8f0f9612b31b862a504cee5b804f160110ba8780faf749bdc2825da5f00123`  
		Last Modified: Wed, 25 Mar 2020 21:33:22 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:latest`

```console
$ docker pull varnish@sha256:c7fbf7c5fa5c5b1ee4b512c0237740136d86551f04c54376c80e7436a47ae994
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:latest` - linux; amd64

```console
$ docker pull varnish@sha256:33901580d26fb83093fe4f5d3bf9dc949c6041054e1148cfae3e8a287af760b1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76767889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b6d153e995c84a2649a50836407ea9ea25a4839102e0755010109b045ce2a9e`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 26 Feb 2020 00:37:39 GMT
ADD file:e5a364615e0f6961626089c7d658adbf8c8d95b3ae95a390a8bb33875317d434 in / 
# Wed, 26 Feb 2020 00:37:39 GMT
CMD ["bash"]
# Wed, 25 Mar 2020 21:32:36 GMT
ENV VARNISH_VERSION=6.4.0-1~buster
# Wed, 25 Mar 2020 21:32:37 GMT
ENV VARNISH_SIZE=100M
# Wed, 25 Mar 2020 21:32:57 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A9897320C397E3A60C03E8BF821AD320F71BFF3D; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish64/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Mar 2020 21:32:57 GMT
WORKDIR /etc/varnish
# Wed, 25 Mar 2020 21:32:57 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Wed, 25 Mar 2020 21:32:57 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 25 Mar 2020 21:32:58 GMT
EXPOSE 80 8443
# Wed, 25 Mar 2020 21:32:58 GMT
CMD []
```

-	Layers:
	-	`sha256:68ced04f60ab5c7a5f1d0b0b4e7572c5a4c8cce44866513d30d9df1a15277d6b`  
		Last Modified: Wed, 26 Feb 2020 00:44:23 GMT  
		Size: 27.1 MB (27091819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9baf6d7f5902865b7612b931e32e7fe4d6c4181522242b5ae5c6a3ef70d6b9`  
		Last Modified: Wed, 25 Mar 2020 21:33:31 GMT  
		Size: 49.7 MB (49675617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8f0f9612b31b862a504cee5b804f160110ba8780faf749bdc2825da5f00123`  
		Last Modified: Wed, 25 Mar 2020 21:33:22 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:stable`

```console
$ docker pull varnish@sha256:c6e4b319a3d57b427dd6c2e362b262da172c49228e7af0693f37a1e15c04efd0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:stable` - linux; amd64

```console
$ docker pull varnish@sha256:acf859b396f9c8643d1a7ec838f034cc2cddaac8ab629996f9451d864a231917
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67208285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e64007059f2bf0a704900b4172bd3c00b82ac9e22aed9b55928a17b21e9cfdf`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 26 Feb 2020 00:41:38 GMT
ADD file:1256c62f77a54c982fdb2790d682049b2ad64c8466466e846f3d33ad1ed4035d in / 
# Wed, 26 Feb 2020 00:41:38 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 20:13:14 GMT
ENV VARNISH_VERSION=6.0.6-1~stretch
# Wed, 25 Mar 2020 21:31:55 GMT
ENV VARNISH_SIZE=100M
# Wed, 25 Mar 2020 21:32:31 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ stretch main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Mar 2020 21:32:31 GMT
WORKDIR /etc/varnish
# Wed, 25 Mar 2020 21:32:32 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Wed, 25 Mar 2020 21:32:32 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Wed, 25 Mar 2020 21:32:32 GMT
EXPOSE 80 8443
# Wed, 25 Mar 2020 21:32:32 GMT
CMD []
```

-	Layers:
	-	`sha256:6d28e14ab8c85bf8a4331de0667c27d19ef4092b12531eec0334b5c2a1012668`  
		Last Modified: Wed, 26 Feb 2020 00:47:21 GMT  
		Size: 22.5 MB (22513365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a559f845f03a758956a7405ece4724da82a6e83566f70bb634b81b3d049232a9`  
		Last Modified: Wed, 25 Mar 2020 21:33:17 GMT  
		Size: 44.7 MB (44694459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148a380b311faddf915d592cd6befeda285bee881c1cee42c2a124891b627239`  
		Last Modified: Wed, 25 Mar 2020 21:33:09 GMT  
		Size: 461.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
