<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `eggdrop`

-	[`eggdrop:1.9`](#eggdrop19)
-	[`eggdrop:1.9.3`](#eggdrop193)
-	[`eggdrop:develop`](#eggdropdevelop)
-	[`eggdrop:latest`](#eggdroplatest)
-	[`eggdrop:stable`](#eggdropstable)

## `eggdrop:1.9`

```console
$ docker pull eggdrop@sha256:7d2100934fc27c2f26a70cc59d32e55fa9ee59c7e6db05cbf5282073c09edf13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:1.9` - linux; amd64

```console
$ docker pull eggdrop@sha256:00977f9e07c4fca52ecb09bdd886c9d1296289eb3f4bc4d34ceb6058280321aa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8185933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68f1c8113271d7672a8598ffcbf230d9554be591c0f2a83a96af68d68739fd02`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 05:20:03 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 12 Nov 2022 05:20:03 GMT
RUN adduser -S eggdrop
# Sat, 12 Nov 2022 05:20:04 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 12 Nov 2022 05:20:06 GMT
RUN apk add --no-cache tcl bash openssl
# Sat, 12 Nov 2022 05:21:01 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gnupg build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.3.tar.gz.asc eggdrop-1.9.3.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.3.tar.gz.asc   && tar -zxvf eggdrop-1.9.3.tar.gz   && rm eggdrop-1.9.3.tar.gz   && ( cd eggdrop-1.9.3     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.3   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 12 Nov 2022 05:21:01 GMT
ENV NICK=
# Sat, 12 Nov 2022 05:21:01 GMT
ENV SERVER=
# Sat, 12 Nov 2022 05:21:01 GMT
ENV LISTEN=3333
# Sat, 12 Nov 2022 05:21:01 GMT
ENV OWNER=
# Sat, 12 Nov 2022 05:21:01 GMT
ENV USERFILE=eggdrop.user
# Sat, 12 Nov 2022 05:21:01 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 12 Nov 2022 05:21:01 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 12 Nov 2022 05:21:01 GMT
EXPOSE 3333
# Sat, 12 Nov 2022 05:21:02 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Sat, 12 Nov 2022 05:21:02 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 12 Nov 2022 05:21:02 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 12 Nov 2022 05:21:02 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cdb365c6f8a662a987df4b9f8aa0a038b4ccf8835a9cf6a10c487d137c48493`  
		Last Modified: Sat, 12 Nov 2022 05:21:21 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc68fd90aec1c649bae31b0426236225d421b45b0010bc88add392ee53e0dcf0`  
		Last Modified: Sat, 12 Nov 2022 05:21:19 GMT  
		Size: 10.9 KB (10938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99cc94fc4b8d42ca4dc27cfd6217256fb76fdab0a0f617ee8f065a731a48c63c`  
		Last Modified: Sat, 12 Nov 2022 05:21:20 GMT  
		Size: 2.8 MB (2757973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3e3a6af178c5f4659f086a81665505442ab8dae18b93cb9e0742dd8fe3a15c`  
		Last Modified: Sat, 12 Nov 2022 05:21:20 GMT  
		Size: 2.6 MB (2606947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9130a261669e0c870a3b64c6113e25b66c235c92ad5b91a3c45cc537f30e995`  
		Last Modified: Sat, 12 Nov 2022 05:21:19 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6456d6a07543b5082e9a76fbd41cc0a2102ce1b230084c9f7e8d01e75a2ad0a`  
		Last Modified: Sat, 12 Nov 2022 05:21:20 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:1.9` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:42b4b4fe83c2326e3f0e2737b6190f2c54f34081f62743c5c71198938e9e713a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7925370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b53198a5c99456ebc6291de898f9ee069a598722ea3ef8bbe4f29dc16c7b670f`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:30:04 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 12 Nov 2022 04:30:04 GMT
RUN adduser -S eggdrop
# Sat, 12 Nov 2022 04:30:05 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 12 Nov 2022 04:30:07 GMT
RUN apk add --no-cache tcl bash openssl
# Sat, 12 Nov 2022 04:31:15 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gnupg build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.3.tar.gz.asc eggdrop-1.9.3.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.3.tar.gz.asc   && tar -zxvf eggdrop-1.9.3.tar.gz   && rm eggdrop-1.9.3.tar.gz   && ( cd eggdrop-1.9.3     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.3   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 12 Nov 2022 04:31:15 GMT
ENV NICK=
# Sat, 12 Nov 2022 04:31:15 GMT
ENV SERVER=
# Sat, 12 Nov 2022 04:31:15 GMT
ENV LISTEN=3333
# Sat, 12 Nov 2022 04:31:15 GMT
ENV OWNER=
# Sat, 12 Nov 2022 04:31:15 GMT
ENV USERFILE=eggdrop.user
# Sat, 12 Nov 2022 04:31:15 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 12 Nov 2022 04:31:15 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 12 Nov 2022 04:31:15 GMT
EXPOSE 3333
# Sat, 12 Nov 2022 04:31:16 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Sat, 12 Nov 2022 04:31:16 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 12 Nov 2022 04:31:16 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 12 Nov 2022 04:31:16 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6634c0ac1b0155242161d0523c05ac568cc7ea7fe315b83be1e9c30a35003815`  
		Last Modified: Sat, 12 Nov 2022 04:31:52 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da2504930a2fea0a18c825055d88cccea76872ba6bb63a0ee3417437e4f9715`  
		Last Modified: Sat, 12 Nov 2022 04:31:50 GMT  
		Size: 10.6 KB (10635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c78cb829fdc1f1248122fcf43eb2d037f10e1e2603b43986980e0f380e4ef5a`  
		Last Modified: Sat, 12 Nov 2022 04:31:51 GMT  
		Size: 2.7 MB (2679712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2faa59e07ead1d75d17d02fcba32516f8eee1aa28132dc62f0901643a819b1b7`  
		Last Modified: Sat, 12 Nov 2022 04:31:51 GMT  
		Size: 2.6 MB (2616139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28613f4f6f8850c15667b7962c813afc082a79e2e25afbc38c2f2ccb31ff5673`  
		Last Modified: Sat, 12 Nov 2022 04:31:50 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff01fbb9b80efa0e93b1da0e94b7d9268327290aec4b8e75b01379b5bf3d788`  
		Last Modified: Sat, 12 Nov 2022 04:31:50 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:1.9` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:ed480444e04df88c2a106e571ea33fce6039ed27604a28ee448f4473fc87efa0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8133123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f9a0e855f2cdcf5d2d90677cba1c7927787eb880e8ff5de17ffd41839d3e5c7`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 06:04:38 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 12 Nov 2022 06:04:38 GMT
RUN adduser -S eggdrop
# Sat, 12 Nov 2022 06:04:39 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 12 Nov 2022 06:04:40 GMT
RUN apk add --no-cache tcl bash openssl
# Sat, 12 Nov 2022 06:05:31 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gnupg build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.3.tar.gz.asc eggdrop-1.9.3.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.3.tar.gz.asc   && tar -zxvf eggdrop-1.9.3.tar.gz   && rm eggdrop-1.9.3.tar.gz   && ( cd eggdrop-1.9.3     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.3   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 12 Nov 2022 06:05:31 GMT
ENV NICK=
# Sat, 12 Nov 2022 06:05:31 GMT
ENV SERVER=
# Sat, 12 Nov 2022 06:05:31 GMT
ENV LISTEN=3333
# Sat, 12 Nov 2022 06:05:31 GMT
ENV OWNER=
# Sat, 12 Nov 2022 06:05:31 GMT
ENV USERFILE=eggdrop.user
# Sat, 12 Nov 2022 06:05:31 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 12 Nov 2022 06:05:31 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 12 Nov 2022 06:05:31 GMT
EXPOSE 3333
# Sat, 12 Nov 2022 06:05:31 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Sat, 12 Nov 2022 06:05:31 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 12 Nov 2022 06:05:31 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 12 Nov 2022 06:05:32 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92c78c1ea1eb5bd99e8235633c5ca1d2a958406fd8a85aac01e596b1ff2417f`  
		Last Modified: Sat, 12 Nov 2022 06:05:48 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e27509a5daaf58faee461c8bfe32ca75c13af7a01476ebd7851958d6fb12f2`  
		Last Modified: Sat, 12 Nov 2022 06:05:45 GMT  
		Size: 10.7 KB (10744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c7e3fd37ee9132ed87bbe8aacd43c174f80d6f6234c8635c3580e0d1146df4`  
		Last Modified: Sat, 12 Nov 2022 06:05:46 GMT  
		Size: 2.8 MB (2776457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285b1f0500c0995c3dc70d3fa8d6c4bb855335616098d2b7448dd566430d8f6a`  
		Last Modified: Sat, 12 Nov 2022 06:05:46 GMT  
		Size: 2.6 MB (2634363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19bb4c740c8e544f42891a0563052575ba6c640ec179444e8ca781d0aec463a`  
		Last Modified: Sat, 12 Nov 2022 06:05:45 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c323895a794adc7bff510a6b7b7dcba0a4bf4349bf3e8d4cd708efb4ac8dde3`  
		Last Modified: Sat, 12 Nov 2022 06:05:45 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:1.9.3`

```console
$ docker pull eggdrop@sha256:7d2100934fc27c2f26a70cc59d32e55fa9ee59c7e6db05cbf5282073c09edf13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:1.9.3` - linux; amd64

```console
$ docker pull eggdrop@sha256:00977f9e07c4fca52ecb09bdd886c9d1296289eb3f4bc4d34ceb6058280321aa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8185933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68f1c8113271d7672a8598ffcbf230d9554be591c0f2a83a96af68d68739fd02`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 05:20:03 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 12 Nov 2022 05:20:03 GMT
RUN adduser -S eggdrop
# Sat, 12 Nov 2022 05:20:04 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 12 Nov 2022 05:20:06 GMT
RUN apk add --no-cache tcl bash openssl
# Sat, 12 Nov 2022 05:21:01 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gnupg build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.3.tar.gz.asc eggdrop-1.9.3.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.3.tar.gz.asc   && tar -zxvf eggdrop-1.9.3.tar.gz   && rm eggdrop-1.9.3.tar.gz   && ( cd eggdrop-1.9.3     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.3   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 12 Nov 2022 05:21:01 GMT
ENV NICK=
# Sat, 12 Nov 2022 05:21:01 GMT
ENV SERVER=
# Sat, 12 Nov 2022 05:21:01 GMT
ENV LISTEN=3333
# Sat, 12 Nov 2022 05:21:01 GMT
ENV OWNER=
# Sat, 12 Nov 2022 05:21:01 GMT
ENV USERFILE=eggdrop.user
# Sat, 12 Nov 2022 05:21:01 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 12 Nov 2022 05:21:01 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 12 Nov 2022 05:21:01 GMT
EXPOSE 3333
# Sat, 12 Nov 2022 05:21:02 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Sat, 12 Nov 2022 05:21:02 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 12 Nov 2022 05:21:02 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 12 Nov 2022 05:21:02 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cdb365c6f8a662a987df4b9f8aa0a038b4ccf8835a9cf6a10c487d137c48493`  
		Last Modified: Sat, 12 Nov 2022 05:21:21 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc68fd90aec1c649bae31b0426236225d421b45b0010bc88add392ee53e0dcf0`  
		Last Modified: Sat, 12 Nov 2022 05:21:19 GMT  
		Size: 10.9 KB (10938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99cc94fc4b8d42ca4dc27cfd6217256fb76fdab0a0f617ee8f065a731a48c63c`  
		Last Modified: Sat, 12 Nov 2022 05:21:20 GMT  
		Size: 2.8 MB (2757973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3e3a6af178c5f4659f086a81665505442ab8dae18b93cb9e0742dd8fe3a15c`  
		Last Modified: Sat, 12 Nov 2022 05:21:20 GMT  
		Size: 2.6 MB (2606947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9130a261669e0c870a3b64c6113e25b66c235c92ad5b91a3c45cc537f30e995`  
		Last Modified: Sat, 12 Nov 2022 05:21:19 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6456d6a07543b5082e9a76fbd41cc0a2102ce1b230084c9f7e8d01e75a2ad0a`  
		Last Modified: Sat, 12 Nov 2022 05:21:20 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:1.9.3` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:42b4b4fe83c2326e3f0e2737b6190f2c54f34081f62743c5c71198938e9e713a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7925370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b53198a5c99456ebc6291de898f9ee069a598722ea3ef8bbe4f29dc16c7b670f`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:30:04 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 12 Nov 2022 04:30:04 GMT
RUN adduser -S eggdrop
# Sat, 12 Nov 2022 04:30:05 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 12 Nov 2022 04:30:07 GMT
RUN apk add --no-cache tcl bash openssl
# Sat, 12 Nov 2022 04:31:15 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gnupg build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.3.tar.gz.asc eggdrop-1.9.3.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.3.tar.gz.asc   && tar -zxvf eggdrop-1.9.3.tar.gz   && rm eggdrop-1.9.3.tar.gz   && ( cd eggdrop-1.9.3     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.3   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 12 Nov 2022 04:31:15 GMT
ENV NICK=
# Sat, 12 Nov 2022 04:31:15 GMT
ENV SERVER=
# Sat, 12 Nov 2022 04:31:15 GMT
ENV LISTEN=3333
# Sat, 12 Nov 2022 04:31:15 GMT
ENV OWNER=
# Sat, 12 Nov 2022 04:31:15 GMT
ENV USERFILE=eggdrop.user
# Sat, 12 Nov 2022 04:31:15 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 12 Nov 2022 04:31:15 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 12 Nov 2022 04:31:15 GMT
EXPOSE 3333
# Sat, 12 Nov 2022 04:31:16 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Sat, 12 Nov 2022 04:31:16 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 12 Nov 2022 04:31:16 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 12 Nov 2022 04:31:16 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6634c0ac1b0155242161d0523c05ac568cc7ea7fe315b83be1e9c30a35003815`  
		Last Modified: Sat, 12 Nov 2022 04:31:52 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da2504930a2fea0a18c825055d88cccea76872ba6bb63a0ee3417437e4f9715`  
		Last Modified: Sat, 12 Nov 2022 04:31:50 GMT  
		Size: 10.6 KB (10635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c78cb829fdc1f1248122fcf43eb2d037f10e1e2603b43986980e0f380e4ef5a`  
		Last Modified: Sat, 12 Nov 2022 04:31:51 GMT  
		Size: 2.7 MB (2679712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2faa59e07ead1d75d17d02fcba32516f8eee1aa28132dc62f0901643a819b1b7`  
		Last Modified: Sat, 12 Nov 2022 04:31:51 GMT  
		Size: 2.6 MB (2616139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28613f4f6f8850c15667b7962c813afc082a79e2e25afbc38c2f2ccb31ff5673`  
		Last Modified: Sat, 12 Nov 2022 04:31:50 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff01fbb9b80efa0e93b1da0e94b7d9268327290aec4b8e75b01379b5bf3d788`  
		Last Modified: Sat, 12 Nov 2022 04:31:50 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:1.9.3` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:ed480444e04df88c2a106e571ea33fce6039ed27604a28ee448f4473fc87efa0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8133123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f9a0e855f2cdcf5d2d90677cba1c7927787eb880e8ff5de17ffd41839d3e5c7`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 06:04:38 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 12 Nov 2022 06:04:38 GMT
RUN adduser -S eggdrop
# Sat, 12 Nov 2022 06:04:39 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 12 Nov 2022 06:04:40 GMT
RUN apk add --no-cache tcl bash openssl
# Sat, 12 Nov 2022 06:05:31 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gnupg build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.3.tar.gz.asc eggdrop-1.9.3.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.3.tar.gz.asc   && tar -zxvf eggdrop-1.9.3.tar.gz   && rm eggdrop-1.9.3.tar.gz   && ( cd eggdrop-1.9.3     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.3   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 12 Nov 2022 06:05:31 GMT
ENV NICK=
# Sat, 12 Nov 2022 06:05:31 GMT
ENV SERVER=
# Sat, 12 Nov 2022 06:05:31 GMT
ENV LISTEN=3333
# Sat, 12 Nov 2022 06:05:31 GMT
ENV OWNER=
# Sat, 12 Nov 2022 06:05:31 GMT
ENV USERFILE=eggdrop.user
# Sat, 12 Nov 2022 06:05:31 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 12 Nov 2022 06:05:31 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 12 Nov 2022 06:05:31 GMT
EXPOSE 3333
# Sat, 12 Nov 2022 06:05:31 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Sat, 12 Nov 2022 06:05:31 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 12 Nov 2022 06:05:31 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 12 Nov 2022 06:05:32 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92c78c1ea1eb5bd99e8235633c5ca1d2a958406fd8a85aac01e596b1ff2417f`  
		Last Modified: Sat, 12 Nov 2022 06:05:48 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e27509a5daaf58faee461c8bfe32ca75c13af7a01476ebd7851958d6fb12f2`  
		Last Modified: Sat, 12 Nov 2022 06:05:45 GMT  
		Size: 10.7 KB (10744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c7e3fd37ee9132ed87bbe8aacd43c174f80d6f6234c8635c3580e0d1146df4`  
		Last Modified: Sat, 12 Nov 2022 06:05:46 GMT  
		Size: 2.8 MB (2776457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285b1f0500c0995c3dc70d3fa8d6c4bb855335616098d2b7448dd566430d8f6a`  
		Last Modified: Sat, 12 Nov 2022 06:05:46 GMT  
		Size: 2.6 MB (2634363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19bb4c740c8e544f42891a0563052575ba6c640ec179444e8ca781d0aec463a`  
		Last Modified: Sat, 12 Nov 2022 06:05:45 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c323895a794adc7bff510a6b7b7dcba0a4bf4349bf3e8d4cd708efb4ac8dde3`  
		Last Modified: Sat, 12 Nov 2022 06:05:45 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:develop`

```console
$ docker pull eggdrop@sha256:6d2d243730b1a6ee39174450f219b775a149373a5e86997f37c2810d292aa408
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:develop` - linux; amd64

```console
$ docker pull eggdrop@sha256:c4ebedf06862c9026d330cdd4338a64d7e3b89490339570140f4e6267a674839
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.7 MB (39697078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d62289e6d48df02c3eccf815833a7761bedd9be6b341e801e799d52395f26ea`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:37:01 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 06 Oct 2022 20:37:02 GMT
RUN adduser -S eggdrop
# Thu, 06 Oct 2022 20:37:03 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 06 Oct 2022 20:37:03 GMT
ENV EGGDROP_SHA256=34915a9bf1870bb3759c68520df62443ba45e01558a53c991d2fb03db9b4ec72
# Thu, 06 Oct 2022 20:37:03 GMT
ENV EGGDROP_COMMIT=47962f7f15a1840b3f3c9ad1a6c247647d16de56
# Thu, 06 Oct 2022 20:37:04 GMT
RUN apk --update add --no-cache bash openssl
# Thu, 06 Oct 2022 20:40:58 GMT
RUN apk --update add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 06 Oct 2022 20:40:58 GMT
ENV NICK=
# Thu, 06 Oct 2022 20:40:58 GMT
ENV SERVER=
# Thu, 06 Oct 2022 20:40:58 GMT
ENV LISTEN=3333
# Thu, 06 Oct 2022 20:40:58 GMT
ENV OWNER=
# Thu, 06 Oct 2022 20:40:59 GMT
ENV USERFILE=eggdrop.user
# Thu, 06 Oct 2022 20:40:59 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 06 Oct 2022 20:40:59 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 06 Oct 2022 20:40:59 GMT
EXPOSE 3333
# Thu, 06 Oct 2022 20:40:59 GMT
COPY file:adf94c8c97044786e05e265ac7a3db4da2f14483f49d1d5b4e825de9c263b6f7 in /home/eggdrop/eggdrop 
# Thu, 06 Oct 2022 20:40:59 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 06 Oct 2022 20:40:59 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 06 Oct 2022 20:40:59 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd629a2e1daaf15d9fdb2bd171b0a8c0622c4f982e7a6b1059c076fb9e1b42e5`  
		Last Modified: Thu, 06 Oct 2022 20:42:28 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dfd741c22df00a71bc308727ead4698aa665f26cbf98ae6e3899b5c94acef40`  
		Last Modified: Thu, 06 Oct 2022 20:42:26 GMT  
		Size: 10.9 KB (10941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964303ee5d62f80866e95b46166f29a7be0468f0e716a1139834084d1207c01b`  
		Last Modified: Thu, 06 Oct 2022 20:42:27 GMT  
		Size: 1.1 MB (1089951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b0e8a3453fdbbc9f5ffc9f8d53a61eea8148a23cd044982b920b601ce44ea3`  
		Last Modified: Thu, 06 Oct 2022 20:42:32 GMT  
		Size: 35.8 MB (35768829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a87c918fc6d1812304b4adb80d63e980cbd841ff7158022764c789c4f4c96c`  
		Last Modified: Thu, 06 Oct 2022 20:42:26 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f63ce19783f457880f6b6b97916947caeb76e4d0f6d0bc8ee04ce17788d9f4`  
		Last Modified: Thu, 06 Oct 2022 20:42:26 GMT  
		Size: 697.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:9e1b2b837053bc99f7eb913a5dfc44f62e0b85cf2d886919ff3572978f53af30
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40323089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cceafd2fe57021f04b81f288eb22eec015c25c22f33c45d1e74ff98a64daed8d`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:36 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Thu, 10 Nov 2022 20:49:36 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:34:46 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 10 Nov 2022 21:34:47 GMT
RUN adduser -S eggdrop
# Thu, 10 Nov 2022 21:34:49 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 10 Nov 2022 21:34:49 GMT
ENV EGGDROP_SHA256=34915a9bf1870bb3759c68520df62443ba45e01558a53c991d2fb03db9b4ec72
# Thu, 10 Nov 2022 21:34:50 GMT
ENV EGGDROP_COMMIT=47962f7f15a1840b3f3c9ad1a6c247647d16de56
# Thu, 10 Nov 2022 21:34:52 GMT
RUN apk --update add --no-cache bash openssl
# Thu, 10 Nov 2022 21:40:31 GMT
RUN apk --update add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 10 Nov 2022 21:40:32 GMT
ENV NICK=
# Thu, 10 Nov 2022 21:40:32 GMT
ENV SERVER=
# Thu, 10 Nov 2022 21:40:33 GMT
ENV LISTEN=3333
# Thu, 10 Nov 2022 21:40:33 GMT
ENV OWNER=
# Thu, 10 Nov 2022 21:40:33 GMT
ENV USERFILE=eggdrop.user
# Thu, 10 Nov 2022 21:40:34 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 10 Nov 2022 21:40:34 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 10 Nov 2022 21:40:34 GMT
EXPOSE 3333
# Thu, 10 Nov 2022 21:40:35 GMT
COPY file:adf94c8c97044786e05e265ac7a3db4da2f14483f49d1d5b4e825de9c263b6f7 in /home/eggdrop/eggdrop 
# Thu, 10 Nov 2022 21:40:36 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 10 Nov 2022 21:40:36 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 10 Nov 2022 21:40:36 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b34cb66db1266899fb04b5d23484182b4fbaeb962888748f7cf45b5469e1cc`  
		Last Modified: Thu, 10 Nov 2022 21:43:03 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b411ce6f41f3486b16f301c44530bcdff2350b1a818209f912759aa06bded636`  
		Last Modified: Thu, 10 Nov 2022 21:43:01 GMT  
		Size: 10.7 KB (10658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb646d185faac53574cfa95136515f08bff42d035401d3dc3a20a8562124ce1`  
		Last Modified: Thu, 10 Nov 2022 21:43:02 GMT  
		Size: 1.0 MB (1032682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1778e52ab4fcc67484c2ada14201eb273d82c5ad36025bf127c9005dd7e2c8`  
		Last Modified: Thu, 10 Nov 2022 21:43:09 GMT  
		Size: 36.6 MB (36644793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d516fa7d1785f6ecb390bad2cdd7c560b7826e17367ba4d88d54e8604f4c893a`  
		Last Modified: Thu, 10 Nov 2022 21:43:01 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce96da4f2fe89372a39bc12c13df40a19bf3ef4a4a79a98c6531ff4f3d6ee80b`  
		Last Modified: Thu, 10 Nov 2022 21:43:01 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:2aa83bbd19a326f4a58611aaf69992a96a217a4cc932f5ec2f45bd6194e30baa
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41110466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30d09e1b0d32b1760d2833069e6397134a5ce6d1846b66f9d1f2e637a4857c13`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 22:03:31 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 10 Nov 2022 22:03:31 GMT
RUN adduser -S eggdrop
# Thu, 10 Nov 2022 22:03:32 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 10 Nov 2022 22:03:32 GMT
ENV EGGDROP_SHA256=34915a9bf1870bb3759c68520df62443ba45e01558a53c991d2fb03db9b4ec72
# Thu, 10 Nov 2022 22:03:32 GMT
ENV EGGDROP_COMMIT=47962f7f15a1840b3f3c9ad1a6c247647d16de56
# Thu, 10 Nov 2022 22:03:33 GMT
RUN apk --update add --no-cache bash openssl
# Thu, 10 Nov 2022 22:07:00 GMT
RUN apk --update add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 10 Nov 2022 22:07:00 GMT
ENV NICK=
# Thu, 10 Nov 2022 22:07:01 GMT
ENV SERVER=
# Thu, 10 Nov 2022 22:07:01 GMT
ENV LISTEN=3333
# Thu, 10 Nov 2022 22:07:01 GMT
ENV OWNER=
# Thu, 10 Nov 2022 22:07:01 GMT
ENV USERFILE=eggdrop.user
# Thu, 10 Nov 2022 22:07:01 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 10 Nov 2022 22:07:01 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 10 Nov 2022 22:07:01 GMT
EXPOSE 3333
# Thu, 10 Nov 2022 22:07:01 GMT
COPY file:adf94c8c97044786e05e265ac7a3db4da2f14483f49d1d5b4e825de9c263b6f7 in /home/eggdrop/eggdrop 
# Thu, 10 Nov 2022 22:07:01 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 10 Nov 2022 22:07:01 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 10 Nov 2022 22:07:01 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0978db877eba00ad9d43a52f1f6b67ecf10580acd57dcecb0bbf56618c8b6c6`  
		Last Modified: Thu, 10 Nov 2022 22:08:28 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70602ff34b989fc029480804413ff335d293fb78a34841211b726953832e7d3d`  
		Last Modified: Thu, 10 Nov 2022 22:08:26 GMT  
		Size: 10.8 KB (10767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1419d1ab26b900f18c1eba3fd137c1f044f6dfcb1450d41f058d89c977d9e97`  
		Last Modified: Thu, 10 Nov 2022 22:08:27 GMT  
		Size: 1.1 MB (1087928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa1d9d534c182fed5115f7a7eff8a08883972f7c0bfe64ddb8181fe9955cc4d`  
		Last Modified: Thu, 10 Nov 2022 22:08:31 GMT  
		Size: 37.3 MB (37289480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845747ce660e3c579fa0582dafc25f48a38f39795b809252b48435b5f2845de2`  
		Last Modified: Thu, 10 Nov 2022 22:08:27 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8623e05f0f2088fd3a32c99ede545a0e1a44429d82b1e52bb239aff77b32f70d`  
		Last Modified: Thu, 10 Nov 2022 22:08:26 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:latest`

```console
$ docker pull eggdrop@sha256:7d2100934fc27c2f26a70cc59d32e55fa9ee59c7e6db05cbf5282073c09edf13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:latest` - linux; amd64

```console
$ docker pull eggdrop@sha256:00977f9e07c4fca52ecb09bdd886c9d1296289eb3f4bc4d34ceb6058280321aa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8185933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68f1c8113271d7672a8598ffcbf230d9554be591c0f2a83a96af68d68739fd02`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 05:20:03 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 12 Nov 2022 05:20:03 GMT
RUN adduser -S eggdrop
# Sat, 12 Nov 2022 05:20:04 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 12 Nov 2022 05:20:06 GMT
RUN apk add --no-cache tcl bash openssl
# Sat, 12 Nov 2022 05:21:01 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gnupg build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.3.tar.gz.asc eggdrop-1.9.3.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.3.tar.gz.asc   && tar -zxvf eggdrop-1.9.3.tar.gz   && rm eggdrop-1.9.3.tar.gz   && ( cd eggdrop-1.9.3     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.3   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 12 Nov 2022 05:21:01 GMT
ENV NICK=
# Sat, 12 Nov 2022 05:21:01 GMT
ENV SERVER=
# Sat, 12 Nov 2022 05:21:01 GMT
ENV LISTEN=3333
# Sat, 12 Nov 2022 05:21:01 GMT
ENV OWNER=
# Sat, 12 Nov 2022 05:21:01 GMT
ENV USERFILE=eggdrop.user
# Sat, 12 Nov 2022 05:21:01 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 12 Nov 2022 05:21:01 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 12 Nov 2022 05:21:01 GMT
EXPOSE 3333
# Sat, 12 Nov 2022 05:21:02 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Sat, 12 Nov 2022 05:21:02 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 12 Nov 2022 05:21:02 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 12 Nov 2022 05:21:02 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cdb365c6f8a662a987df4b9f8aa0a038b4ccf8835a9cf6a10c487d137c48493`  
		Last Modified: Sat, 12 Nov 2022 05:21:21 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc68fd90aec1c649bae31b0426236225d421b45b0010bc88add392ee53e0dcf0`  
		Last Modified: Sat, 12 Nov 2022 05:21:19 GMT  
		Size: 10.9 KB (10938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99cc94fc4b8d42ca4dc27cfd6217256fb76fdab0a0f617ee8f065a731a48c63c`  
		Last Modified: Sat, 12 Nov 2022 05:21:20 GMT  
		Size: 2.8 MB (2757973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3e3a6af178c5f4659f086a81665505442ab8dae18b93cb9e0742dd8fe3a15c`  
		Last Modified: Sat, 12 Nov 2022 05:21:20 GMT  
		Size: 2.6 MB (2606947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9130a261669e0c870a3b64c6113e25b66c235c92ad5b91a3c45cc537f30e995`  
		Last Modified: Sat, 12 Nov 2022 05:21:19 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6456d6a07543b5082e9a76fbd41cc0a2102ce1b230084c9f7e8d01e75a2ad0a`  
		Last Modified: Sat, 12 Nov 2022 05:21:20 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:latest` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:42b4b4fe83c2326e3f0e2737b6190f2c54f34081f62743c5c71198938e9e713a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7925370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b53198a5c99456ebc6291de898f9ee069a598722ea3ef8bbe4f29dc16c7b670f`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:30:04 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 12 Nov 2022 04:30:04 GMT
RUN adduser -S eggdrop
# Sat, 12 Nov 2022 04:30:05 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 12 Nov 2022 04:30:07 GMT
RUN apk add --no-cache tcl bash openssl
# Sat, 12 Nov 2022 04:31:15 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gnupg build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.3.tar.gz.asc eggdrop-1.9.3.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.3.tar.gz.asc   && tar -zxvf eggdrop-1.9.3.tar.gz   && rm eggdrop-1.9.3.tar.gz   && ( cd eggdrop-1.9.3     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.3   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 12 Nov 2022 04:31:15 GMT
ENV NICK=
# Sat, 12 Nov 2022 04:31:15 GMT
ENV SERVER=
# Sat, 12 Nov 2022 04:31:15 GMT
ENV LISTEN=3333
# Sat, 12 Nov 2022 04:31:15 GMT
ENV OWNER=
# Sat, 12 Nov 2022 04:31:15 GMT
ENV USERFILE=eggdrop.user
# Sat, 12 Nov 2022 04:31:15 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 12 Nov 2022 04:31:15 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 12 Nov 2022 04:31:15 GMT
EXPOSE 3333
# Sat, 12 Nov 2022 04:31:16 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Sat, 12 Nov 2022 04:31:16 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 12 Nov 2022 04:31:16 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 12 Nov 2022 04:31:16 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6634c0ac1b0155242161d0523c05ac568cc7ea7fe315b83be1e9c30a35003815`  
		Last Modified: Sat, 12 Nov 2022 04:31:52 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da2504930a2fea0a18c825055d88cccea76872ba6bb63a0ee3417437e4f9715`  
		Last Modified: Sat, 12 Nov 2022 04:31:50 GMT  
		Size: 10.6 KB (10635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c78cb829fdc1f1248122fcf43eb2d037f10e1e2603b43986980e0f380e4ef5a`  
		Last Modified: Sat, 12 Nov 2022 04:31:51 GMT  
		Size: 2.7 MB (2679712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2faa59e07ead1d75d17d02fcba32516f8eee1aa28132dc62f0901643a819b1b7`  
		Last Modified: Sat, 12 Nov 2022 04:31:51 GMT  
		Size: 2.6 MB (2616139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28613f4f6f8850c15667b7962c813afc082a79e2e25afbc38c2f2ccb31ff5673`  
		Last Modified: Sat, 12 Nov 2022 04:31:50 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff01fbb9b80efa0e93b1da0e94b7d9268327290aec4b8e75b01379b5bf3d788`  
		Last Modified: Sat, 12 Nov 2022 04:31:50 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:latest` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:ed480444e04df88c2a106e571ea33fce6039ed27604a28ee448f4473fc87efa0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8133123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f9a0e855f2cdcf5d2d90677cba1c7927787eb880e8ff5de17ffd41839d3e5c7`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 06:04:38 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 12 Nov 2022 06:04:38 GMT
RUN adduser -S eggdrop
# Sat, 12 Nov 2022 06:04:39 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 12 Nov 2022 06:04:40 GMT
RUN apk add --no-cache tcl bash openssl
# Sat, 12 Nov 2022 06:05:31 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gnupg build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.3.tar.gz.asc eggdrop-1.9.3.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.3.tar.gz.asc   && tar -zxvf eggdrop-1.9.3.tar.gz   && rm eggdrop-1.9.3.tar.gz   && ( cd eggdrop-1.9.3     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.3   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 12 Nov 2022 06:05:31 GMT
ENV NICK=
# Sat, 12 Nov 2022 06:05:31 GMT
ENV SERVER=
# Sat, 12 Nov 2022 06:05:31 GMT
ENV LISTEN=3333
# Sat, 12 Nov 2022 06:05:31 GMT
ENV OWNER=
# Sat, 12 Nov 2022 06:05:31 GMT
ENV USERFILE=eggdrop.user
# Sat, 12 Nov 2022 06:05:31 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 12 Nov 2022 06:05:31 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 12 Nov 2022 06:05:31 GMT
EXPOSE 3333
# Sat, 12 Nov 2022 06:05:31 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Sat, 12 Nov 2022 06:05:31 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 12 Nov 2022 06:05:31 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 12 Nov 2022 06:05:32 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92c78c1ea1eb5bd99e8235633c5ca1d2a958406fd8a85aac01e596b1ff2417f`  
		Last Modified: Sat, 12 Nov 2022 06:05:48 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e27509a5daaf58faee461c8bfe32ca75c13af7a01476ebd7851958d6fb12f2`  
		Last Modified: Sat, 12 Nov 2022 06:05:45 GMT  
		Size: 10.7 KB (10744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c7e3fd37ee9132ed87bbe8aacd43c174f80d6f6234c8635c3580e0d1146df4`  
		Last Modified: Sat, 12 Nov 2022 06:05:46 GMT  
		Size: 2.8 MB (2776457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285b1f0500c0995c3dc70d3fa8d6c4bb855335616098d2b7448dd566430d8f6a`  
		Last Modified: Sat, 12 Nov 2022 06:05:46 GMT  
		Size: 2.6 MB (2634363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19bb4c740c8e544f42891a0563052575ba6c640ec179444e8ca781d0aec463a`  
		Last Modified: Sat, 12 Nov 2022 06:05:45 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c323895a794adc7bff510a6b7b7dcba0a4bf4349bf3e8d4cd708efb4ac8dde3`  
		Last Modified: Sat, 12 Nov 2022 06:05:45 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:stable`

```console
$ docker pull eggdrop@sha256:7d2100934fc27c2f26a70cc59d32e55fa9ee59c7e6db05cbf5282073c09edf13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:stable` - linux; amd64

```console
$ docker pull eggdrop@sha256:00977f9e07c4fca52ecb09bdd886c9d1296289eb3f4bc4d34ceb6058280321aa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8185933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68f1c8113271d7672a8598ffcbf230d9554be591c0f2a83a96af68d68739fd02`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 05:20:03 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 12 Nov 2022 05:20:03 GMT
RUN adduser -S eggdrop
# Sat, 12 Nov 2022 05:20:04 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 12 Nov 2022 05:20:06 GMT
RUN apk add --no-cache tcl bash openssl
# Sat, 12 Nov 2022 05:21:01 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gnupg build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.3.tar.gz.asc eggdrop-1.9.3.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.3.tar.gz.asc   && tar -zxvf eggdrop-1.9.3.tar.gz   && rm eggdrop-1.9.3.tar.gz   && ( cd eggdrop-1.9.3     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.3   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 12 Nov 2022 05:21:01 GMT
ENV NICK=
# Sat, 12 Nov 2022 05:21:01 GMT
ENV SERVER=
# Sat, 12 Nov 2022 05:21:01 GMT
ENV LISTEN=3333
# Sat, 12 Nov 2022 05:21:01 GMT
ENV OWNER=
# Sat, 12 Nov 2022 05:21:01 GMT
ENV USERFILE=eggdrop.user
# Sat, 12 Nov 2022 05:21:01 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 12 Nov 2022 05:21:01 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 12 Nov 2022 05:21:01 GMT
EXPOSE 3333
# Sat, 12 Nov 2022 05:21:02 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Sat, 12 Nov 2022 05:21:02 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 12 Nov 2022 05:21:02 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 12 Nov 2022 05:21:02 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cdb365c6f8a662a987df4b9f8aa0a038b4ccf8835a9cf6a10c487d137c48493`  
		Last Modified: Sat, 12 Nov 2022 05:21:21 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc68fd90aec1c649bae31b0426236225d421b45b0010bc88add392ee53e0dcf0`  
		Last Modified: Sat, 12 Nov 2022 05:21:19 GMT  
		Size: 10.9 KB (10938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99cc94fc4b8d42ca4dc27cfd6217256fb76fdab0a0f617ee8f065a731a48c63c`  
		Last Modified: Sat, 12 Nov 2022 05:21:20 GMT  
		Size: 2.8 MB (2757973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3e3a6af178c5f4659f086a81665505442ab8dae18b93cb9e0742dd8fe3a15c`  
		Last Modified: Sat, 12 Nov 2022 05:21:20 GMT  
		Size: 2.6 MB (2606947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9130a261669e0c870a3b64c6113e25b66c235c92ad5b91a3c45cc537f30e995`  
		Last Modified: Sat, 12 Nov 2022 05:21:19 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6456d6a07543b5082e9a76fbd41cc0a2102ce1b230084c9f7e8d01e75a2ad0a`  
		Last Modified: Sat, 12 Nov 2022 05:21:20 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:stable` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:42b4b4fe83c2326e3f0e2737b6190f2c54f34081f62743c5c71198938e9e713a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7925370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b53198a5c99456ebc6291de898f9ee069a598722ea3ef8bbe4f29dc16c7b670f`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:30:04 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 12 Nov 2022 04:30:04 GMT
RUN adduser -S eggdrop
# Sat, 12 Nov 2022 04:30:05 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 12 Nov 2022 04:30:07 GMT
RUN apk add --no-cache tcl bash openssl
# Sat, 12 Nov 2022 04:31:15 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gnupg build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.3.tar.gz.asc eggdrop-1.9.3.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.3.tar.gz.asc   && tar -zxvf eggdrop-1.9.3.tar.gz   && rm eggdrop-1.9.3.tar.gz   && ( cd eggdrop-1.9.3     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.3   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 12 Nov 2022 04:31:15 GMT
ENV NICK=
# Sat, 12 Nov 2022 04:31:15 GMT
ENV SERVER=
# Sat, 12 Nov 2022 04:31:15 GMT
ENV LISTEN=3333
# Sat, 12 Nov 2022 04:31:15 GMT
ENV OWNER=
# Sat, 12 Nov 2022 04:31:15 GMT
ENV USERFILE=eggdrop.user
# Sat, 12 Nov 2022 04:31:15 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 12 Nov 2022 04:31:15 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 12 Nov 2022 04:31:15 GMT
EXPOSE 3333
# Sat, 12 Nov 2022 04:31:16 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Sat, 12 Nov 2022 04:31:16 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 12 Nov 2022 04:31:16 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 12 Nov 2022 04:31:16 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6634c0ac1b0155242161d0523c05ac568cc7ea7fe315b83be1e9c30a35003815`  
		Last Modified: Sat, 12 Nov 2022 04:31:52 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da2504930a2fea0a18c825055d88cccea76872ba6bb63a0ee3417437e4f9715`  
		Last Modified: Sat, 12 Nov 2022 04:31:50 GMT  
		Size: 10.6 KB (10635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c78cb829fdc1f1248122fcf43eb2d037f10e1e2603b43986980e0f380e4ef5a`  
		Last Modified: Sat, 12 Nov 2022 04:31:51 GMT  
		Size: 2.7 MB (2679712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2faa59e07ead1d75d17d02fcba32516f8eee1aa28132dc62f0901643a819b1b7`  
		Last Modified: Sat, 12 Nov 2022 04:31:51 GMT  
		Size: 2.6 MB (2616139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28613f4f6f8850c15667b7962c813afc082a79e2e25afbc38c2f2ccb31ff5673`  
		Last Modified: Sat, 12 Nov 2022 04:31:50 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff01fbb9b80efa0e93b1da0e94b7d9268327290aec4b8e75b01379b5bf3d788`  
		Last Modified: Sat, 12 Nov 2022 04:31:50 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:stable` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:ed480444e04df88c2a106e571ea33fce6039ed27604a28ee448f4473fc87efa0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8133123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f9a0e855f2cdcf5d2d90677cba1c7927787eb880e8ff5de17ffd41839d3e5c7`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 06:04:38 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 12 Nov 2022 06:04:38 GMT
RUN adduser -S eggdrop
# Sat, 12 Nov 2022 06:04:39 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 12 Nov 2022 06:04:40 GMT
RUN apk add --no-cache tcl bash openssl
# Sat, 12 Nov 2022 06:05:31 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gnupg build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.3.tar.gz.asc eggdrop-1.9.3.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.3.tar.gz.asc   && tar -zxvf eggdrop-1.9.3.tar.gz   && rm eggdrop-1.9.3.tar.gz   && ( cd eggdrop-1.9.3     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.3   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 12 Nov 2022 06:05:31 GMT
ENV NICK=
# Sat, 12 Nov 2022 06:05:31 GMT
ENV SERVER=
# Sat, 12 Nov 2022 06:05:31 GMT
ENV LISTEN=3333
# Sat, 12 Nov 2022 06:05:31 GMT
ENV OWNER=
# Sat, 12 Nov 2022 06:05:31 GMT
ENV USERFILE=eggdrop.user
# Sat, 12 Nov 2022 06:05:31 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 12 Nov 2022 06:05:31 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 12 Nov 2022 06:05:31 GMT
EXPOSE 3333
# Sat, 12 Nov 2022 06:05:31 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Sat, 12 Nov 2022 06:05:31 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 12 Nov 2022 06:05:31 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 12 Nov 2022 06:05:32 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92c78c1ea1eb5bd99e8235633c5ca1d2a958406fd8a85aac01e596b1ff2417f`  
		Last Modified: Sat, 12 Nov 2022 06:05:48 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e27509a5daaf58faee461c8bfe32ca75c13af7a01476ebd7851958d6fb12f2`  
		Last Modified: Sat, 12 Nov 2022 06:05:45 GMT  
		Size: 10.7 KB (10744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c7e3fd37ee9132ed87bbe8aacd43c174f80d6f6234c8635c3580e0d1146df4`  
		Last Modified: Sat, 12 Nov 2022 06:05:46 GMT  
		Size: 2.8 MB (2776457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285b1f0500c0995c3dc70d3fa8d6c4bb855335616098d2b7448dd566430d8f6a`  
		Last Modified: Sat, 12 Nov 2022 06:05:46 GMT  
		Size: 2.6 MB (2634363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19bb4c740c8e544f42891a0563052575ba6c640ec179444e8ca781d0aec463a`  
		Last Modified: Sat, 12 Nov 2022 06:05:45 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c323895a794adc7bff510a6b7b7dcba0a4bf4349bf3e8d4cd708efb4ac8dde3`  
		Last Modified: Sat, 12 Nov 2022 06:05:45 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
