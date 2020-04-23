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
$ docker pull varnish@sha256:b6adc2db657ec6120661a1d6c395bce501cc3449d13596cf380f6fb8b7df46ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6` - linux; amd64

```console
$ docker pull varnish@sha256:4a3cef85679a3e2b6f4ff34b421f91db431fd835f7a6661134886a06cbfb2f58
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76774316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58fb7a9b0b998257bd2088de0b526d304c2efa3b754d73c478579c9862301bb6`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 19:09:45 GMT
ENV VARNISH_VERSION=6.4.0-1~buster
# Thu, 23 Apr 2020 19:09:45 GMT
ENV VARNISH_SIZE=100M
# Thu, 23 Apr 2020 19:10:12 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A9897320C397E3A60C03E8BF821AD320F71BFF3D; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish64/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 19:10:12 GMT
WORKDIR /etc/varnish
# Thu, 23 Apr 2020 19:10:12 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Thu, 23 Apr 2020 19:10:13 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Thu, 23 Apr 2020 19:10:13 GMT
EXPOSE 80 8443
# Thu, 23 Apr 2020 19:10:13 GMT
CMD []
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9679bef917109b4df69e4e3303870b8b8a9824689236a57d32610c5dc018a6`  
		Last Modified: Thu, 23 Apr 2020 19:10:51 GMT  
		Size: 49.7 MB (49675609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c71288eaf0af463539b07d00291749ee7e4349ba5b00371a4c2382213e823cc`  
		Last Modified: Thu, 23 Apr 2020 19:10:40 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0`

```console
$ docker pull varnish@sha256:23dbce6557dccbc644942a1d20cb09788a5b3c0dbd4697ca1228171e4b49ae54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.0` - linux; amd64

```console
$ docker pull varnish@sha256:7620b65d641312b0f67c082b91158ef33f693027c253d739f9f2cf4c1fb057f6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67208494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:198e5462c4fbd7ef0018d50ae5717e7ceff0d6bd30370926ddfbb2cc6871c54d`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Apr 2020 00:23:03 GMT
ADD file:08ea1ff3fcd4efc24ab4f262cfa24e55e65844f6858e41a46fe0635d247f174d in / 
# Thu, 23 Apr 2020 00:23:03 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 19:09:05 GMT
ENV VARNISH_VERSION=6.0.6-1~stretch
# Thu, 23 Apr 2020 19:09:05 GMT
ENV VARNISH_SIZE=100M
# Thu, 23 Apr 2020 19:09:35 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ stretch main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 19:09:36 GMT
WORKDIR /etc/varnish
# Thu, 23 Apr 2020 19:09:36 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Thu, 23 Apr 2020 19:09:36 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Thu, 23 Apr 2020 19:09:36 GMT
EXPOSE 80 8443
# Thu, 23 Apr 2020 19:09:37 GMT
CMD []
```

-	Layers:
	-	`sha256:b248fa9f6d2ae427ad7f00de3537ab256ae7eb413565f8be0773ee9b86ef57d4`  
		Last Modified: Thu, 23 Apr 2020 00:27:46 GMT  
		Size: 22.5 MB (22513488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5144e1c776d778942d57fc51127cdaab19af3b4715d4d4eaf1d193df54ed5666`  
		Last Modified: Thu, 23 Apr 2020 19:10:34 GMT  
		Size: 44.7 MB (44694544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b84f51e99b9f925b18b5cf67ccd4b9fdd4c461ced9e474d75c9df14b01e74d`  
		Last Modified: Thu, 23 Apr 2020 19:10:24 GMT  
		Size: 462.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0.6`

```console
$ docker pull varnish@sha256:23dbce6557dccbc644942a1d20cb09788a5b3c0dbd4697ca1228171e4b49ae54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.0.6` - linux; amd64

```console
$ docker pull varnish@sha256:7620b65d641312b0f67c082b91158ef33f693027c253d739f9f2cf4c1fb057f6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67208494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:198e5462c4fbd7ef0018d50ae5717e7ceff0d6bd30370926ddfbb2cc6871c54d`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Apr 2020 00:23:03 GMT
ADD file:08ea1ff3fcd4efc24ab4f262cfa24e55e65844f6858e41a46fe0635d247f174d in / 
# Thu, 23 Apr 2020 00:23:03 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 19:09:05 GMT
ENV VARNISH_VERSION=6.0.6-1~stretch
# Thu, 23 Apr 2020 19:09:05 GMT
ENV VARNISH_SIZE=100M
# Thu, 23 Apr 2020 19:09:35 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ stretch main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 19:09:36 GMT
WORKDIR /etc/varnish
# Thu, 23 Apr 2020 19:09:36 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Thu, 23 Apr 2020 19:09:36 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Thu, 23 Apr 2020 19:09:36 GMT
EXPOSE 80 8443
# Thu, 23 Apr 2020 19:09:37 GMT
CMD []
```

-	Layers:
	-	`sha256:b248fa9f6d2ae427ad7f00de3537ab256ae7eb413565f8be0773ee9b86ef57d4`  
		Last Modified: Thu, 23 Apr 2020 00:27:46 GMT  
		Size: 22.5 MB (22513488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5144e1c776d778942d57fc51127cdaab19af3b4715d4d4eaf1d193df54ed5666`  
		Last Modified: Thu, 23 Apr 2020 19:10:34 GMT  
		Size: 44.7 MB (44694544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b84f51e99b9f925b18b5cf67ccd4b9fdd4c461ced9e474d75c9df14b01e74d`  
		Last Modified: Thu, 23 Apr 2020 19:10:24 GMT  
		Size: 462.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0.6-1`

```console
$ docker pull varnish@sha256:23dbce6557dccbc644942a1d20cb09788a5b3c0dbd4697ca1228171e4b49ae54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.0.6-1` - linux; amd64

```console
$ docker pull varnish@sha256:7620b65d641312b0f67c082b91158ef33f693027c253d739f9f2cf4c1fb057f6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67208494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:198e5462c4fbd7ef0018d50ae5717e7ceff0d6bd30370926ddfbb2cc6871c54d`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Apr 2020 00:23:03 GMT
ADD file:08ea1ff3fcd4efc24ab4f262cfa24e55e65844f6858e41a46fe0635d247f174d in / 
# Thu, 23 Apr 2020 00:23:03 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 19:09:05 GMT
ENV VARNISH_VERSION=6.0.6-1~stretch
# Thu, 23 Apr 2020 19:09:05 GMT
ENV VARNISH_SIZE=100M
# Thu, 23 Apr 2020 19:09:35 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ stretch main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 19:09:36 GMT
WORKDIR /etc/varnish
# Thu, 23 Apr 2020 19:09:36 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Thu, 23 Apr 2020 19:09:36 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Thu, 23 Apr 2020 19:09:36 GMT
EXPOSE 80 8443
# Thu, 23 Apr 2020 19:09:37 GMT
CMD []
```

-	Layers:
	-	`sha256:b248fa9f6d2ae427ad7f00de3537ab256ae7eb413565f8be0773ee9b86ef57d4`  
		Last Modified: Thu, 23 Apr 2020 00:27:46 GMT  
		Size: 22.5 MB (22513488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5144e1c776d778942d57fc51127cdaab19af3b4715d4d4eaf1d193df54ed5666`  
		Last Modified: Thu, 23 Apr 2020 19:10:34 GMT  
		Size: 44.7 MB (44694544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b84f51e99b9f925b18b5cf67ccd4b9fdd4c461ced9e474d75c9df14b01e74d`  
		Last Modified: Thu, 23 Apr 2020 19:10:24 GMT  
		Size: 462.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.4`

```console
$ docker pull varnish@sha256:b6adc2db657ec6120661a1d6c395bce501cc3449d13596cf380f6fb8b7df46ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.4` - linux; amd64

```console
$ docker pull varnish@sha256:4a3cef85679a3e2b6f4ff34b421f91db431fd835f7a6661134886a06cbfb2f58
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76774316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58fb7a9b0b998257bd2088de0b526d304c2efa3b754d73c478579c9862301bb6`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 19:09:45 GMT
ENV VARNISH_VERSION=6.4.0-1~buster
# Thu, 23 Apr 2020 19:09:45 GMT
ENV VARNISH_SIZE=100M
# Thu, 23 Apr 2020 19:10:12 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A9897320C397E3A60C03E8BF821AD320F71BFF3D; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish64/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 19:10:12 GMT
WORKDIR /etc/varnish
# Thu, 23 Apr 2020 19:10:12 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Thu, 23 Apr 2020 19:10:13 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Thu, 23 Apr 2020 19:10:13 GMT
EXPOSE 80 8443
# Thu, 23 Apr 2020 19:10:13 GMT
CMD []
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9679bef917109b4df69e4e3303870b8b8a9824689236a57d32610c5dc018a6`  
		Last Modified: Thu, 23 Apr 2020 19:10:51 GMT  
		Size: 49.7 MB (49675609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c71288eaf0af463539b07d00291749ee7e4349ba5b00371a4c2382213e823cc`  
		Last Modified: Thu, 23 Apr 2020 19:10:40 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.4.0`

```console
$ docker pull varnish@sha256:b6adc2db657ec6120661a1d6c395bce501cc3449d13596cf380f6fb8b7df46ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.4.0` - linux; amd64

```console
$ docker pull varnish@sha256:4a3cef85679a3e2b6f4ff34b421f91db431fd835f7a6661134886a06cbfb2f58
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76774316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58fb7a9b0b998257bd2088de0b526d304c2efa3b754d73c478579c9862301bb6`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 19:09:45 GMT
ENV VARNISH_VERSION=6.4.0-1~buster
# Thu, 23 Apr 2020 19:09:45 GMT
ENV VARNISH_SIZE=100M
# Thu, 23 Apr 2020 19:10:12 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A9897320C397E3A60C03E8BF821AD320F71BFF3D; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish64/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 19:10:12 GMT
WORKDIR /etc/varnish
# Thu, 23 Apr 2020 19:10:12 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Thu, 23 Apr 2020 19:10:13 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Thu, 23 Apr 2020 19:10:13 GMT
EXPOSE 80 8443
# Thu, 23 Apr 2020 19:10:13 GMT
CMD []
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9679bef917109b4df69e4e3303870b8b8a9824689236a57d32610c5dc018a6`  
		Last Modified: Thu, 23 Apr 2020 19:10:51 GMT  
		Size: 49.7 MB (49675609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c71288eaf0af463539b07d00291749ee7e4349ba5b00371a4c2382213e823cc`  
		Last Modified: Thu, 23 Apr 2020 19:10:40 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.4.0-1`

```console
$ docker pull varnish@sha256:b6adc2db657ec6120661a1d6c395bce501cc3449d13596cf380f6fb8b7df46ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:6.4.0-1` - linux; amd64

```console
$ docker pull varnish@sha256:4a3cef85679a3e2b6f4ff34b421f91db431fd835f7a6661134886a06cbfb2f58
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76774316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58fb7a9b0b998257bd2088de0b526d304c2efa3b754d73c478579c9862301bb6`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 19:09:45 GMT
ENV VARNISH_VERSION=6.4.0-1~buster
# Thu, 23 Apr 2020 19:09:45 GMT
ENV VARNISH_SIZE=100M
# Thu, 23 Apr 2020 19:10:12 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A9897320C397E3A60C03E8BF821AD320F71BFF3D; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish64/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 19:10:12 GMT
WORKDIR /etc/varnish
# Thu, 23 Apr 2020 19:10:12 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Thu, 23 Apr 2020 19:10:13 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Thu, 23 Apr 2020 19:10:13 GMT
EXPOSE 80 8443
# Thu, 23 Apr 2020 19:10:13 GMT
CMD []
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9679bef917109b4df69e4e3303870b8b8a9824689236a57d32610c5dc018a6`  
		Last Modified: Thu, 23 Apr 2020 19:10:51 GMT  
		Size: 49.7 MB (49675609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c71288eaf0af463539b07d00291749ee7e4349ba5b00371a4c2382213e823cc`  
		Last Modified: Thu, 23 Apr 2020 19:10:40 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:fresh`

```console
$ docker pull varnish@sha256:b6adc2db657ec6120661a1d6c395bce501cc3449d13596cf380f6fb8b7df46ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:fresh` - linux; amd64

```console
$ docker pull varnish@sha256:4a3cef85679a3e2b6f4ff34b421f91db431fd835f7a6661134886a06cbfb2f58
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76774316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58fb7a9b0b998257bd2088de0b526d304c2efa3b754d73c478579c9862301bb6`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 19:09:45 GMT
ENV VARNISH_VERSION=6.4.0-1~buster
# Thu, 23 Apr 2020 19:09:45 GMT
ENV VARNISH_SIZE=100M
# Thu, 23 Apr 2020 19:10:12 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A9897320C397E3A60C03E8BF821AD320F71BFF3D; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish64/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 19:10:12 GMT
WORKDIR /etc/varnish
# Thu, 23 Apr 2020 19:10:12 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Thu, 23 Apr 2020 19:10:13 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Thu, 23 Apr 2020 19:10:13 GMT
EXPOSE 80 8443
# Thu, 23 Apr 2020 19:10:13 GMT
CMD []
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9679bef917109b4df69e4e3303870b8b8a9824689236a57d32610c5dc018a6`  
		Last Modified: Thu, 23 Apr 2020 19:10:51 GMT  
		Size: 49.7 MB (49675609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c71288eaf0af463539b07d00291749ee7e4349ba5b00371a4c2382213e823cc`  
		Last Modified: Thu, 23 Apr 2020 19:10:40 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:latest`

```console
$ docker pull varnish@sha256:b6adc2db657ec6120661a1d6c395bce501cc3449d13596cf380f6fb8b7df46ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:latest` - linux; amd64

```console
$ docker pull varnish@sha256:4a3cef85679a3e2b6f4ff34b421f91db431fd835f7a6661134886a06cbfb2f58
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76774316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58fb7a9b0b998257bd2088de0b526d304c2efa3b754d73c478579c9862301bb6`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 19:09:45 GMT
ENV VARNISH_VERSION=6.4.0-1~buster
# Thu, 23 Apr 2020 19:09:45 GMT
ENV VARNISH_SIZE=100M
# Thu, 23 Apr 2020 19:10:12 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=A9897320C397E3A60C03E8BF821AD320F71BFF3D; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish64/debian/ buster main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 19:10:12 GMT
WORKDIR /etc/varnish
# Thu, 23 Apr 2020 19:10:12 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Thu, 23 Apr 2020 19:10:13 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Thu, 23 Apr 2020 19:10:13 GMT
EXPOSE 80 8443
# Thu, 23 Apr 2020 19:10:13 GMT
CMD []
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9679bef917109b4df69e4e3303870b8b8a9824689236a57d32610c5dc018a6`  
		Last Modified: Thu, 23 Apr 2020 19:10:51 GMT  
		Size: 49.7 MB (49675609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c71288eaf0af463539b07d00291749ee7e4349ba5b00371a4c2382213e823cc`  
		Last Modified: Thu, 23 Apr 2020 19:10:40 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:stable`

```console
$ docker pull varnish@sha256:23dbce6557dccbc644942a1d20cb09788a5b3c0dbd4697ca1228171e4b49ae54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `varnish:stable` - linux; amd64

```console
$ docker pull varnish@sha256:7620b65d641312b0f67c082b91158ef33f693027c253d739f9f2cf4c1fb057f6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67208494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:198e5462c4fbd7ef0018d50ae5717e7ceff0d6bd30370926ddfbb2cc6871c54d`
-	Entrypoint: `["docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Apr 2020 00:23:03 GMT
ADD file:08ea1ff3fcd4efc24ab4f262cfa24e55e65844f6858e41a46fe0635d247f174d in / 
# Thu, 23 Apr 2020 00:23:03 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 19:09:05 GMT
ENV VARNISH_VERSION=6.0.6-1~stretch
# Thu, 23 Apr 2020 19:09:05 GMT
ENV VARNISH_SIZE=100M
# Thu, 23 Apr 2020 19:09:35 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends apt-transport-https ca-certificates $fetchDeps; 	key=48D81A24CB0456F5D59431D94CFCFD6BA750EDCD; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://hkps.pool.sks-keyservers.net --recv-keys $key; 	gpg --batch --export export $key > /etc/apt/trusted.gpg.d/varnish.gpg; 	gpgconf --kill all; 	rm -rf $GNUPGHOME; 	echo deb https://packagecloud.io/varnishcache/varnish60lts/debian/ stretch main > /etc/apt/sources.list.d/varnish.list; 	apt-get update; 	apt-get install -y --no-install-recommends varnish=$VARNISH_VERSION; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 19:09:36 GMT
WORKDIR /etc/varnish
# Thu, 23 Apr 2020 19:09:36 GMT
COPY file:4156d91450dca54febf2b6908a0871cf84271dba1069d9641be798ec9f560393 in /usr/local/bin/ 
# Thu, 23 Apr 2020 19:09:36 GMT
ENTRYPOINT ["docker-varnish-entrypoint"]
# Thu, 23 Apr 2020 19:09:36 GMT
EXPOSE 80 8443
# Thu, 23 Apr 2020 19:09:37 GMT
CMD []
```

-	Layers:
	-	`sha256:b248fa9f6d2ae427ad7f00de3537ab256ae7eb413565f8be0773ee9b86ef57d4`  
		Last Modified: Thu, 23 Apr 2020 00:27:46 GMT  
		Size: 22.5 MB (22513488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5144e1c776d778942d57fc51127cdaab19af3b4715d4d4eaf1d193df54ed5666`  
		Last Modified: Thu, 23 Apr 2020 19:10:34 GMT  
		Size: 44.7 MB (44694544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b84f51e99b9f925b18b5cf67ccd4b9fdd4c461ced9e474d75c9df14b01e74d`  
		Last Modified: Thu, 23 Apr 2020 19:10:24 GMT  
		Size: 462.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
