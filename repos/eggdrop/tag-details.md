<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `eggdrop`

-	[`eggdrop:1.8`](#eggdrop18)
-	[`eggdrop:1.8.4`](#eggdrop184)
-	[`eggdrop:1.9`](#eggdrop19)
-	[`eggdrop:1.9.1`](#eggdrop191)
-	[`eggdrop:develop`](#eggdropdevelop)
-	[`eggdrop:latest`](#eggdroplatest)
-	[`eggdrop:stable`](#eggdropstable)

## `eggdrop:1.8`

```console
$ docker pull eggdrop@sha256:20e9e88de9ad7aaa3c7d6beb98dbd5b2c2ed6b4863847bee489b020ec035b4c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `eggdrop:1.8` - linux; amd64

```console
$ docker pull eggdrop@sha256:3515bc8d05ff6214c16fa920bd27f66468844e616e114a44a9c5968cc810adff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8801912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:158d1a7aca7e5a2c0c5e721c885f80379ad74b38e0f936d81f764950730c8b58`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:31 GMT
ADD file:9d14b11183983923090d9e6d15cc51ee210466296e913bfefbfd580b3de59c95 in / 
# Tue, 31 Aug 2021 23:18:31 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:45:26 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 01 Sep 2021 00:45:27 GMT
RUN adduser -S eggdrop
# Wed, 01 Sep 2021 00:45:29 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 01 Sep 2021 00:47:24 GMT
RUN apk add --no-cache tcl bash openssl
# Wed, 01 Sep 2021 00:48:53 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.4.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.4.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.8.4.tar.gz.asc eggdrop-1.8.4.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.8.4.tar.gz.asc   && tar -zxvf eggdrop-1.8.4.tar.gz   && rm eggdrop-1.8.4.tar.gz   && ( cd eggdrop-1.8.4     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.8.4   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 01 Sep 2021 00:48:54 GMT
ENV NICK=
# Wed, 01 Sep 2021 00:48:54 GMT
ENV SERVER=
# Wed, 01 Sep 2021 00:48:54 GMT
ENV LISTEN=3333
# Wed, 01 Sep 2021 00:48:55 GMT
ENV OWNER=
# Wed, 01 Sep 2021 00:48:55 GMT
ENV USERFILE=eggdrop.user
# Wed, 01 Sep 2021 00:48:55 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 01 Sep 2021 00:48:56 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 01 Sep 2021 00:48:56 GMT
EXPOSE 3333
# Wed, 01 Sep 2021 00:48:57 GMT
COPY file:f8d85155d39ecdefdd2ce710ca8c1211edaffb7c3fbbde0877da166dd3aaa579 in /home/eggdrop/eggdrop 
# Wed, 01 Sep 2021 00:48:57 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 01 Sep 2021 00:48:58 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 01 Sep 2021 00:48:58 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:6a428f9f83b0a29f1fdd2ccccca19a9bab805a925b8eddf432a5a3d3da04afbc`  
		Last Modified: Tue, 31 Aug 2021 23:19:15 GMT  
		Size: 2.8 MB (2817307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f20f9fdd96b050b7674a3c80fab08aa90a03ade7cdb1605902daa948fda52a2`  
		Last Modified: Wed, 01 Sep 2021 00:50:59 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20bd70c5c8eea46f41315a10333d6c4180d7330668d5d9a03a677e69f00dc72e`  
		Last Modified: Wed, 01 Sep 2021 00:50:56 GMT  
		Size: 9.6 KB (9603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2574265c46e1bcf9b75a096f4c4ba73e414b625819aed53a53f373e11e016dc`  
		Last Modified: Wed, 01 Sep 2021 00:51:07 GMT  
		Size: 2.7 MB (2685358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c786a5b4be16b348ab37d1166a4e4c7d64fb1c801787034e017600ff03553208`  
		Last Modified: Wed, 01 Sep 2021 00:51:07 GMT  
		Size: 3.3 MB (3285797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f54e33975937b1852cb665d7c706121b1e18b1182d603de1f5dc8c9ed981e7`  
		Last Modified: Wed, 01 Sep 2021 00:51:06 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf6541232161c3bb1d26a43c96019ab8d7689d531648c648bb4d7125d21ae39`  
		Last Modified: Wed, 01 Sep 2021 00:51:06 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:1.8.4`

```console
$ docker pull eggdrop@sha256:20e9e88de9ad7aaa3c7d6beb98dbd5b2c2ed6b4863847bee489b020ec035b4c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `eggdrop:1.8.4` - linux; amd64

```console
$ docker pull eggdrop@sha256:3515bc8d05ff6214c16fa920bd27f66468844e616e114a44a9c5968cc810adff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8801912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:158d1a7aca7e5a2c0c5e721c885f80379ad74b38e0f936d81f764950730c8b58`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:31 GMT
ADD file:9d14b11183983923090d9e6d15cc51ee210466296e913bfefbfd580b3de59c95 in / 
# Tue, 31 Aug 2021 23:18:31 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:45:26 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 01 Sep 2021 00:45:27 GMT
RUN adduser -S eggdrop
# Wed, 01 Sep 2021 00:45:29 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 01 Sep 2021 00:47:24 GMT
RUN apk add --no-cache tcl bash openssl
# Wed, 01 Sep 2021 00:48:53 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.4.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.4.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.8.4.tar.gz.asc eggdrop-1.8.4.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.8.4.tar.gz.asc   && tar -zxvf eggdrop-1.8.4.tar.gz   && rm eggdrop-1.8.4.tar.gz   && ( cd eggdrop-1.8.4     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.8.4   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 01 Sep 2021 00:48:54 GMT
ENV NICK=
# Wed, 01 Sep 2021 00:48:54 GMT
ENV SERVER=
# Wed, 01 Sep 2021 00:48:54 GMT
ENV LISTEN=3333
# Wed, 01 Sep 2021 00:48:55 GMT
ENV OWNER=
# Wed, 01 Sep 2021 00:48:55 GMT
ENV USERFILE=eggdrop.user
# Wed, 01 Sep 2021 00:48:55 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 01 Sep 2021 00:48:56 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 01 Sep 2021 00:48:56 GMT
EXPOSE 3333
# Wed, 01 Sep 2021 00:48:57 GMT
COPY file:f8d85155d39ecdefdd2ce710ca8c1211edaffb7c3fbbde0877da166dd3aaa579 in /home/eggdrop/eggdrop 
# Wed, 01 Sep 2021 00:48:57 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 01 Sep 2021 00:48:58 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 01 Sep 2021 00:48:58 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:6a428f9f83b0a29f1fdd2ccccca19a9bab805a925b8eddf432a5a3d3da04afbc`  
		Last Modified: Tue, 31 Aug 2021 23:19:15 GMT  
		Size: 2.8 MB (2817307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f20f9fdd96b050b7674a3c80fab08aa90a03ade7cdb1605902daa948fda52a2`  
		Last Modified: Wed, 01 Sep 2021 00:50:59 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20bd70c5c8eea46f41315a10333d6c4180d7330668d5d9a03a677e69f00dc72e`  
		Last Modified: Wed, 01 Sep 2021 00:50:56 GMT  
		Size: 9.6 KB (9603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2574265c46e1bcf9b75a096f4c4ba73e414b625819aed53a53f373e11e016dc`  
		Last Modified: Wed, 01 Sep 2021 00:51:07 GMT  
		Size: 2.7 MB (2685358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c786a5b4be16b348ab37d1166a4e4c7d64fb1c801787034e017600ff03553208`  
		Last Modified: Wed, 01 Sep 2021 00:51:07 GMT  
		Size: 3.3 MB (3285797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f54e33975937b1852cb665d7c706121b1e18b1182d603de1f5dc8c9ed981e7`  
		Last Modified: Wed, 01 Sep 2021 00:51:06 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf6541232161c3bb1d26a43c96019ab8d7689d531648c648bb4d7125d21ae39`  
		Last Modified: Wed, 01 Sep 2021 00:51:06 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:1.9`

```console
$ docker pull eggdrop@sha256:da791d7beb860dc9067745220f3f6d0437003c4fc7014b1256c367cf85405d48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:1.9` - linux; amd64

```console
$ docker pull eggdrop@sha256:6e892a67931479b599c272a667e2938484206e52d7264ff14d7b7db016f37b30
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8289929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15447097e0374d1ea165db47231adde6fb63ff6480b16f30134b7a313a3b43e9`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:49:03 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 01 Sep 2021 00:49:05 GMT
RUN adduser -S eggdrop
# Wed, 01 Sep 2021 00:49:07 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 01 Sep 2021 00:49:10 GMT
RUN apk add --no-cache tcl bash openssl
# Wed, 01 Sep 2021 00:50:26 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.1.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.1.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.1.tar.gz.asc eggdrop-1.9.1.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.1.tar.gz.asc   && tar -zxvf eggdrop-1.9.1.tar.gz   && rm eggdrop-1.9.1.tar.gz   && ( cd eggdrop-1.9.1     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.1   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 01 Sep 2021 00:50:26 GMT
ENV NICK=
# Wed, 01 Sep 2021 00:50:27 GMT
ENV SERVER=
# Wed, 01 Sep 2021 00:50:27 GMT
ENV LISTEN=3333
# Wed, 01 Sep 2021 00:50:27 GMT
ENV OWNER=
# Wed, 01 Sep 2021 00:50:27 GMT
ENV USERFILE=eggdrop.user
# Wed, 01 Sep 2021 00:50:27 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 01 Sep 2021 00:50:28 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 01 Sep 2021 00:50:28 GMT
EXPOSE 3333
# Wed, 01 Sep 2021 00:50:28 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Wed, 01 Sep 2021 00:50:28 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 01 Sep 2021 00:50:29 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 01 Sep 2021 00:50:29 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2739640d4bb626124033590fe2bf187a76c1f09fc23aa7686e7c3fab1ea81d84`  
		Last Modified: Wed, 01 Sep 2021 00:51:19 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738ab5f4a6a9c53e0f6ed425003f94b60df8ec4e166993682419cfe0a94a62f5`  
		Last Modified: Wed, 01 Sep 2021 00:51:16 GMT  
		Size: 10.1 KB (10118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0880ee1cbcc03493b50e3d163c452ce2bbb7b3de40bf0f955c9744388500b821`  
		Last Modified: Wed, 01 Sep 2021 00:51:17 GMT  
		Size: 2.7 MB (2724823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734b1d2617820fb511e667242f74784e1a91e810da7643c518373cea683dc9f5`  
		Last Modified: Wed, 01 Sep 2021 00:51:17 GMT  
		Size: 2.7 MB (2737114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2384c732a6a65e03999103c3cb481f0e361b99732133b52e23f57be3a24759`  
		Last Modified: Wed, 01 Sep 2021 00:51:16 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4ab1d804e5474fe3998c40986e14f69650bea83115a3f78da3e35a49da8219`  
		Last Modified: Wed, 01 Sep 2021 00:51:16 GMT  
		Size: 698.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:1.9` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:256bf1e8371ae1436bd7b27b318801ba886744ed2a1225293f5d586fac79f541
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7984703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c777347de3a39dff1a465be9c70eeda9ba5de814025ba8d418620d17956a5a7b`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Tue, 31 Aug 2021 22:30:33 GMT
ADD file:ed2b5e0fbd1e7ae37ab8f808c827d23c6841ce1edd7427552d5bf741d67ebcc0 in / 
# Tue, 31 Aug 2021 22:30:33 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 01:40:18 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 01 Sep 2021 01:40:20 GMT
RUN adduser -S eggdrop
# Wed, 01 Sep 2021 01:40:22 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 01 Sep 2021 01:40:25 GMT
RUN apk add --no-cache tcl bash openssl
# Wed, 01 Sep 2021 01:42:54 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.1.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.1.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.1.tar.gz.asc eggdrop-1.9.1.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.1.tar.gz.asc   && tar -zxvf eggdrop-1.9.1.tar.gz   && rm eggdrop-1.9.1.tar.gz   && ( cd eggdrop-1.9.1     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.1   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 01 Sep 2021 01:42:54 GMT
ENV NICK=
# Wed, 01 Sep 2021 01:42:55 GMT
ENV SERVER=
# Wed, 01 Sep 2021 01:42:55 GMT
ENV LISTEN=3333
# Wed, 01 Sep 2021 01:42:56 GMT
ENV OWNER=
# Wed, 01 Sep 2021 01:42:56 GMT
ENV USERFILE=eggdrop.user
# Wed, 01 Sep 2021 01:42:56 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 01 Sep 2021 01:42:57 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 01 Sep 2021 01:42:57 GMT
EXPOSE 3333
# Wed, 01 Sep 2021 01:42:58 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Wed, 01 Sep 2021 01:42:58 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 01 Sep 2021 01:42:59 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 01 Sep 2021 01:42:59 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:840d18d84f6afdc3231d126fdd3f84f23f0335b61cbfa9cb8808b888a4308919`  
		Last Modified: Tue, 31 Aug 2021 22:32:11 GMT  
		Size: 2.6 MB (2623761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f046c2415fb1127f8d46523c533c6d2cce3bd492e0d68c48c260d220336ca952`  
		Last Modified: Wed, 01 Sep 2021 01:43:59 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf336ff3aa2db3f62c40723c1adc70b28e83510d2314cff15dcb5e218e1c2af`  
		Last Modified: Wed, 01 Sep 2021 01:43:57 GMT  
		Size: 9.8 KB (9833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87713f793a04367c6610fc1476e6a6f31d2e474ebb4598fde28a9728dbd06ae`  
		Last Modified: Wed, 01 Sep 2021 01:43:59 GMT  
		Size: 2.7 MB (2652189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7192b1f59b63dc171f423af626fa69dc717358b1645dd0db5b1ed1fb3cbbb2bc`  
		Last Modified: Wed, 01 Sep 2021 01:43:59 GMT  
		Size: 2.7 MB (2695121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c74d83e6f19d90b93b685a87dd4c0c1b522bc2338d4fe8c56b9806a195ca45`  
		Last Modified: Wed, 01 Sep 2021 01:43:57 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6402fc12bd28bda7948b0b77e3a48bd0ebb3f7d2ce610b45949fcfc92e8e478a`  
		Last Modified: Wed, 01 Sep 2021 01:43:57 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:1.9` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:bff7cdffd49712f662b1cde3d2375d386b65b1d3e7a9d91df91436e887bb32cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8210746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d1b5ae8312bcd75a3d6d7db1867b4f7070e3b7ed4e1ca97549a9e3c9f5d577f`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 15:15:36 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 01 Sep 2021 15:15:37 GMT
RUN adduser -S eggdrop
# Wed, 01 Sep 2021 15:15:38 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 01 Sep 2021 15:15:40 GMT
RUN apk add --no-cache tcl bash openssl
# Wed, 01 Sep 2021 15:16:52 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.1.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.1.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.1.tar.gz.asc eggdrop-1.9.1.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.1.tar.gz.asc   && tar -zxvf eggdrop-1.9.1.tar.gz   && rm eggdrop-1.9.1.tar.gz   && ( cd eggdrop-1.9.1     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.1   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 01 Sep 2021 15:16:52 GMT
ENV NICK=
# Wed, 01 Sep 2021 15:16:52 GMT
ENV SERVER=
# Wed, 01 Sep 2021 15:16:53 GMT
ENV LISTEN=3333
# Wed, 01 Sep 2021 15:16:53 GMT
ENV OWNER=
# Wed, 01 Sep 2021 15:16:53 GMT
ENV USERFILE=eggdrop.user
# Wed, 01 Sep 2021 15:16:53 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 01 Sep 2021 15:16:53 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 01 Sep 2021 15:16:53 GMT
EXPOSE 3333
# Wed, 01 Sep 2021 15:16:54 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Wed, 01 Sep 2021 15:16:54 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 01 Sep 2021 15:16:54 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 01 Sep 2021 15:16:54 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf67b3e836d0edeb34044ffda17873e401619019ce483f22005e430bc1433d4`  
		Last Modified: Wed, 01 Sep 2021 15:17:30 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b59c6abd4c336393a25dbe734281b04d79212c90032285294352d9d3f78958e`  
		Last Modified: Wed, 01 Sep 2021 15:17:28 GMT  
		Size: 10.0 KB (9995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae931fd0b19febff0674f2c50c3aa65d9c43ba202ee949c3de1aec49d6546c5e`  
		Last Modified: Wed, 01 Sep 2021 15:17:28 GMT  
		Size: 2.8 MB (2752469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5521e7d97fa85dd2c1c5040eedc8afdcd905ffddf8eae87dcdecc9d1a950b4e6`  
		Last Modified: Wed, 01 Sep 2021 15:17:28 GMT  
		Size: 2.7 MB (2731473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517861ca5ee30a5ce6da73542fdb0b2cbdfdf1bb73d813e0e39e8bdd9f0ce77e`  
		Last Modified: Wed, 01 Sep 2021 15:17:28 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2278cfa27b2d9e72ddec10cbe8092918ff164b9f10a6b6a0356017b49a94ba`  
		Last Modified: Wed, 01 Sep 2021 15:17:28 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:1.9.1`

```console
$ docker pull eggdrop@sha256:da791d7beb860dc9067745220f3f6d0437003c4fc7014b1256c367cf85405d48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:1.9.1` - linux; amd64

```console
$ docker pull eggdrop@sha256:6e892a67931479b599c272a667e2938484206e52d7264ff14d7b7db016f37b30
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8289929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15447097e0374d1ea165db47231adde6fb63ff6480b16f30134b7a313a3b43e9`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:49:03 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 01 Sep 2021 00:49:05 GMT
RUN adduser -S eggdrop
# Wed, 01 Sep 2021 00:49:07 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 01 Sep 2021 00:49:10 GMT
RUN apk add --no-cache tcl bash openssl
# Wed, 01 Sep 2021 00:50:26 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.1.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.1.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.1.tar.gz.asc eggdrop-1.9.1.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.1.tar.gz.asc   && tar -zxvf eggdrop-1.9.1.tar.gz   && rm eggdrop-1.9.1.tar.gz   && ( cd eggdrop-1.9.1     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.1   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 01 Sep 2021 00:50:26 GMT
ENV NICK=
# Wed, 01 Sep 2021 00:50:27 GMT
ENV SERVER=
# Wed, 01 Sep 2021 00:50:27 GMT
ENV LISTEN=3333
# Wed, 01 Sep 2021 00:50:27 GMT
ENV OWNER=
# Wed, 01 Sep 2021 00:50:27 GMT
ENV USERFILE=eggdrop.user
# Wed, 01 Sep 2021 00:50:27 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 01 Sep 2021 00:50:28 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 01 Sep 2021 00:50:28 GMT
EXPOSE 3333
# Wed, 01 Sep 2021 00:50:28 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Wed, 01 Sep 2021 00:50:28 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 01 Sep 2021 00:50:29 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 01 Sep 2021 00:50:29 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2739640d4bb626124033590fe2bf187a76c1f09fc23aa7686e7c3fab1ea81d84`  
		Last Modified: Wed, 01 Sep 2021 00:51:19 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738ab5f4a6a9c53e0f6ed425003f94b60df8ec4e166993682419cfe0a94a62f5`  
		Last Modified: Wed, 01 Sep 2021 00:51:16 GMT  
		Size: 10.1 KB (10118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0880ee1cbcc03493b50e3d163c452ce2bbb7b3de40bf0f955c9744388500b821`  
		Last Modified: Wed, 01 Sep 2021 00:51:17 GMT  
		Size: 2.7 MB (2724823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734b1d2617820fb511e667242f74784e1a91e810da7643c518373cea683dc9f5`  
		Last Modified: Wed, 01 Sep 2021 00:51:17 GMT  
		Size: 2.7 MB (2737114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2384c732a6a65e03999103c3cb481f0e361b99732133b52e23f57be3a24759`  
		Last Modified: Wed, 01 Sep 2021 00:51:16 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4ab1d804e5474fe3998c40986e14f69650bea83115a3f78da3e35a49da8219`  
		Last Modified: Wed, 01 Sep 2021 00:51:16 GMT  
		Size: 698.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:1.9.1` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:256bf1e8371ae1436bd7b27b318801ba886744ed2a1225293f5d586fac79f541
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7984703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c777347de3a39dff1a465be9c70eeda9ba5de814025ba8d418620d17956a5a7b`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Tue, 31 Aug 2021 22:30:33 GMT
ADD file:ed2b5e0fbd1e7ae37ab8f808c827d23c6841ce1edd7427552d5bf741d67ebcc0 in / 
# Tue, 31 Aug 2021 22:30:33 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 01:40:18 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 01 Sep 2021 01:40:20 GMT
RUN adduser -S eggdrop
# Wed, 01 Sep 2021 01:40:22 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 01 Sep 2021 01:40:25 GMT
RUN apk add --no-cache tcl bash openssl
# Wed, 01 Sep 2021 01:42:54 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.1.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.1.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.1.tar.gz.asc eggdrop-1.9.1.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.1.tar.gz.asc   && tar -zxvf eggdrop-1.9.1.tar.gz   && rm eggdrop-1.9.1.tar.gz   && ( cd eggdrop-1.9.1     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.1   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 01 Sep 2021 01:42:54 GMT
ENV NICK=
# Wed, 01 Sep 2021 01:42:55 GMT
ENV SERVER=
# Wed, 01 Sep 2021 01:42:55 GMT
ENV LISTEN=3333
# Wed, 01 Sep 2021 01:42:56 GMT
ENV OWNER=
# Wed, 01 Sep 2021 01:42:56 GMT
ENV USERFILE=eggdrop.user
# Wed, 01 Sep 2021 01:42:56 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 01 Sep 2021 01:42:57 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 01 Sep 2021 01:42:57 GMT
EXPOSE 3333
# Wed, 01 Sep 2021 01:42:58 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Wed, 01 Sep 2021 01:42:58 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 01 Sep 2021 01:42:59 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 01 Sep 2021 01:42:59 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:840d18d84f6afdc3231d126fdd3f84f23f0335b61cbfa9cb8808b888a4308919`  
		Last Modified: Tue, 31 Aug 2021 22:32:11 GMT  
		Size: 2.6 MB (2623761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f046c2415fb1127f8d46523c533c6d2cce3bd492e0d68c48c260d220336ca952`  
		Last Modified: Wed, 01 Sep 2021 01:43:59 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf336ff3aa2db3f62c40723c1adc70b28e83510d2314cff15dcb5e218e1c2af`  
		Last Modified: Wed, 01 Sep 2021 01:43:57 GMT  
		Size: 9.8 KB (9833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87713f793a04367c6610fc1476e6a6f31d2e474ebb4598fde28a9728dbd06ae`  
		Last Modified: Wed, 01 Sep 2021 01:43:59 GMT  
		Size: 2.7 MB (2652189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7192b1f59b63dc171f423af626fa69dc717358b1645dd0db5b1ed1fb3cbbb2bc`  
		Last Modified: Wed, 01 Sep 2021 01:43:59 GMT  
		Size: 2.7 MB (2695121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c74d83e6f19d90b93b685a87dd4c0c1b522bc2338d4fe8c56b9806a195ca45`  
		Last Modified: Wed, 01 Sep 2021 01:43:57 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6402fc12bd28bda7948b0b77e3a48bd0ebb3f7d2ce610b45949fcfc92e8e478a`  
		Last Modified: Wed, 01 Sep 2021 01:43:57 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:1.9.1` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:bff7cdffd49712f662b1cde3d2375d386b65b1d3e7a9d91df91436e887bb32cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8210746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d1b5ae8312bcd75a3d6d7db1867b4f7070e3b7ed4e1ca97549a9e3c9f5d577f`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 15:15:36 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 01 Sep 2021 15:15:37 GMT
RUN adduser -S eggdrop
# Wed, 01 Sep 2021 15:15:38 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 01 Sep 2021 15:15:40 GMT
RUN apk add --no-cache tcl bash openssl
# Wed, 01 Sep 2021 15:16:52 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.1.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.1.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.1.tar.gz.asc eggdrop-1.9.1.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.1.tar.gz.asc   && tar -zxvf eggdrop-1.9.1.tar.gz   && rm eggdrop-1.9.1.tar.gz   && ( cd eggdrop-1.9.1     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.1   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 01 Sep 2021 15:16:52 GMT
ENV NICK=
# Wed, 01 Sep 2021 15:16:52 GMT
ENV SERVER=
# Wed, 01 Sep 2021 15:16:53 GMT
ENV LISTEN=3333
# Wed, 01 Sep 2021 15:16:53 GMT
ENV OWNER=
# Wed, 01 Sep 2021 15:16:53 GMT
ENV USERFILE=eggdrop.user
# Wed, 01 Sep 2021 15:16:53 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 01 Sep 2021 15:16:53 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 01 Sep 2021 15:16:53 GMT
EXPOSE 3333
# Wed, 01 Sep 2021 15:16:54 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Wed, 01 Sep 2021 15:16:54 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 01 Sep 2021 15:16:54 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 01 Sep 2021 15:16:54 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf67b3e836d0edeb34044ffda17873e401619019ce483f22005e430bc1433d4`  
		Last Modified: Wed, 01 Sep 2021 15:17:30 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b59c6abd4c336393a25dbe734281b04d79212c90032285294352d9d3f78958e`  
		Last Modified: Wed, 01 Sep 2021 15:17:28 GMT  
		Size: 10.0 KB (9995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae931fd0b19febff0674f2c50c3aa65d9c43ba202ee949c3de1aec49d6546c5e`  
		Last Modified: Wed, 01 Sep 2021 15:17:28 GMT  
		Size: 2.8 MB (2752469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5521e7d97fa85dd2c1c5040eedc8afdcd905ffddf8eae87dcdecc9d1a950b4e6`  
		Last Modified: Wed, 01 Sep 2021 15:17:28 GMT  
		Size: 2.7 MB (2731473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517861ca5ee30a5ce6da73542fdb0b2cbdfdf1bb73d813e0e39e8bdd9f0ce77e`  
		Last Modified: Wed, 01 Sep 2021 15:17:28 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2278cfa27b2d9e72ddec10cbe8092918ff164b9f10a6b6a0356017b49a94ba`  
		Last Modified: Wed, 01 Sep 2021 15:17:28 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:develop`

```console
$ docker pull eggdrop@sha256:9a6eb9a85e0b7a37587d595fe990ea3e04d060d587603d9ade07c3b0ece8dbae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:develop` - linux; amd64

```console
$ docker pull eggdrop@sha256:ac51c0945714354a18de779773d2a06aea0eba1a5db4f39a59afa998af0f2d54
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (13971126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b18f8406444915774df8bc7fde6cb77d2d7cfdb1f8efbd11c34dfcd931fa42e4`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Fri, 12 Nov 2021 17:20:17 GMT
ADD file:efe2d94a88cdbbd01c3ef095f0a2473cec9e74804b49cd6fb9b837d362631409 in / 
# Fri, 12 Nov 2021 17:20:17 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 22:16:40 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Fri, 12 Nov 2021 22:16:42 GMT
RUN adduser -S eggdrop
# Fri, 12 Nov 2021 22:16:44 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Fri, 12 Nov 2021 22:16:44 GMT
ENV EGGDROP_SHA256=f977f8f586d1b65d2bae581b5b5828d79193a29a217f617c4c74d1868a566c7f
# Fri, 12 Nov 2021 22:16:45 GMT
ENV EGGDROP_COMMIT=886c2ff6f943952018000c16cb48c08b8ab99127
# Fri, 12 Nov 2021 22:16:48 GMT
RUN apk --update add --no-cache tcl bash openssl
# Fri, 12 Nov 2021 22:18:15 GMT
RUN apk --update add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256  develop.tar.gz" | sha256sum -c -   && tar -zxvf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Fri, 12 Nov 2021 22:18:15 GMT
ENV NICK=
# Fri, 12 Nov 2021 22:18:15 GMT
ENV SERVER=
# Fri, 12 Nov 2021 22:18:16 GMT
ENV LISTEN=3333
# Fri, 12 Nov 2021 22:18:16 GMT
ENV OWNER=
# Fri, 12 Nov 2021 22:18:16 GMT
ENV USERFILE=eggdrop.user
# Fri, 12 Nov 2021 22:18:16 GMT
ENV CHANFILE=eggdrop.chan
# Fri, 12 Nov 2021 22:18:17 GMT
WORKDIR /home/eggdrop/eggdrop
# Fri, 12 Nov 2021 22:18:17 GMT
EXPOSE 3333
# Fri, 12 Nov 2021 22:18:17 GMT
COPY file:adf94c8c97044786e05e265ac7a3db4da2f14483f49d1d5b4e825de9c263b6f7 in /home/eggdrop/eggdrop 
# Fri, 12 Nov 2021 22:18:17 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Fri, 12 Nov 2021 22:18:17 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Fri, 12 Nov 2021 22:18:18 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:79e9f2f55bf5465a02ee6a6170e66005b20c7aa6b115af6fcd04fad706ea651a`  
		Last Modified: Fri, 12 Nov 2021 17:21:24 GMT  
		Size: 2.8 MB (2817409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81adda6e9eba444737eb924c547e315175df5a0ce22872ddefa8d3e84e6d8426`  
		Last Modified: Fri, 12 Nov 2021 23:38:59 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c6691f36cfa95bda1f875a9e50901e42545817a24e6fd9cb8463d931f68075`  
		Last Modified: Fri, 12 Nov 2021 23:38:57 GMT  
		Size: 9.6 KB (9592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1745cf1ed4da7a73fcd90fbf3034e047ac1ddcfc9cafd47e6bec219875fd02b9`  
		Last Modified: Fri, 12 Nov 2021 23:38:57 GMT  
		Size: 2.7 MB (2685370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df75c7a1bacde78f2df7ea75d7a042759a70bdc1a2e64625cf00980990a9b4da`  
		Last Modified: Fri, 12 Nov 2021 23:38:58 GMT  
		Size: 8.5 MB (8454906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3a328dd9ff12c659f26cf5675153e3f8cfd0d2b31419e4d27dac84638dc1cd`  
		Last Modified: Fri, 12 Nov 2021 23:38:57 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb35aaa19b161c31605b0557e35b5f89b077501a6006bf5d840e6cfc255fa07e`  
		Last Modified: Fri, 12 Nov 2021 23:38:56 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:04f5da1f8d9cfe9b4de20d07b8aaf6580c423e499b7aa1f92c3efd19ce804d9e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13629131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5248e64648b70dd2a8aecf181dad16c62e9d8e29e1a0c849d51461bd31028895`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Fri, 12 Nov 2021 16:50:22 GMT
ADD file:c219ee7662a2b29c4e06be5bf332f2f53b326937277057af61516f5cf5abce1e in / 
# Fri, 12 Nov 2021 16:50:23 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 03:30:49 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 13 Nov 2021 03:30:51 GMT
RUN adduser -S eggdrop
# Sat, 13 Nov 2021 03:30:53 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 13 Nov 2021 03:30:53 GMT
ENV EGGDROP_SHA256=f977f8f586d1b65d2bae581b5b5828d79193a29a217f617c4c74d1868a566c7f
# Sat, 13 Nov 2021 03:30:54 GMT
ENV EGGDROP_COMMIT=886c2ff6f943952018000c16cb48c08b8ab99127
# Sat, 13 Nov 2021 03:30:57 GMT
RUN apk --update add --no-cache tcl bash openssl
# Sat, 13 Nov 2021 03:33:19 GMT
RUN apk --update add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256  develop.tar.gz" | sha256sum -c -   && tar -zxvf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 13 Nov 2021 03:33:19 GMT
ENV NICK=
# Sat, 13 Nov 2021 03:33:20 GMT
ENV SERVER=
# Sat, 13 Nov 2021 03:33:20 GMT
ENV LISTEN=3333
# Sat, 13 Nov 2021 03:33:21 GMT
ENV OWNER=
# Sat, 13 Nov 2021 03:33:21 GMT
ENV USERFILE=eggdrop.user
# Sat, 13 Nov 2021 03:33:21 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 13 Nov 2021 03:33:22 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 13 Nov 2021 03:33:22 GMT
EXPOSE 3333
# Sat, 13 Nov 2021 03:33:23 GMT
COPY file:adf94c8c97044786e05e265ac7a3db4da2f14483f49d1d5b4e825de9c263b6f7 in /home/eggdrop/eggdrop 
# Sat, 13 Nov 2021 03:33:23 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 13 Nov 2021 03:33:24 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 13 Nov 2021 03:33:24 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:5cb8b15578b20b3c847454a0e0743b923ddea3e4f22ffa95f6f41b0c551a391e`  
		Last Modified: Fri, 12 Nov 2021 16:52:20 GMT  
		Size: 2.6 MB (2623510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c9647b4c3050e47077e5c8d9edce7ae926c3eefafc735a6d81ae469a024c07`  
		Last Modified: Sat, 13 Nov 2021 05:53:01 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c37ba58553c63fd2ebdb5da2016f7c19934d0142773987afbdcf01d6ab27b8`  
		Last Modified: Sat, 13 Nov 2021 05:52:59 GMT  
		Size: 9.4 KB (9401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8db5f2e7b2aaa5174a81b283f2169f8b8bdb1541e83f9627eac970e7d131e4`  
		Last Modified: Sat, 13 Nov 2021 05:53:01 GMT  
		Size: 2.6 MB (2608749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d2918d67befd1ef0a53c4a262000402dc37d2319db48ac355ea31e3329d37c`  
		Last Modified: Sat, 13 Nov 2021 05:53:03 GMT  
		Size: 8.4 MB (8383622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03c6c6a8ac6c10a942eac56504eafae00725f92eb42b53619939705d3e43ddb`  
		Last Modified: Sat, 13 Nov 2021 05:52:59 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ddd2315eb1df07d63a69e2844cb7573ea7737fa3222e8f4fb6943a11ddf4e21`  
		Last Modified: Sat, 13 Nov 2021 05:52:59 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:b082575f3b7776a35592d8b1e4fc81b7e46d43715fb16bf1667d4240b8bbddcd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13933506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:709c2cd43aab5d0a0aef27eaf5ed741a05accc39b4127c91f1f572013ae33b80`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:19 GMT
ADD file:bffb4828c6bba0115b766f72c49407938059b204ac9edf130d023af34871d3d0 in / 
# Fri, 12 Nov 2021 16:40:19 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 08:51:17 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 13 Nov 2021 08:51:18 GMT
RUN adduser -S eggdrop
# Sat, 13 Nov 2021 08:51:19 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 13 Nov 2021 08:51:20 GMT
ENV EGGDROP_SHA256=f977f8f586d1b65d2bae581b5b5828d79193a29a217f617c4c74d1868a566c7f
# Sat, 13 Nov 2021 08:51:21 GMT
ENV EGGDROP_COMMIT=886c2ff6f943952018000c16cb48c08b8ab99127
# Sat, 13 Nov 2021 08:51:23 GMT
RUN apk --update add --no-cache tcl bash openssl
# Sat, 13 Nov 2021 08:52:22 GMT
RUN apk --update add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256  develop.tar.gz" | sha256sum -c -   && tar -zxvf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 13 Nov 2021 08:52:22 GMT
ENV NICK=
# Sat, 13 Nov 2021 08:52:23 GMT
ENV SERVER=
# Sat, 13 Nov 2021 08:52:24 GMT
ENV LISTEN=3333
# Sat, 13 Nov 2021 08:52:25 GMT
ENV OWNER=
# Sat, 13 Nov 2021 08:52:26 GMT
ENV USERFILE=eggdrop.user
# Sat, 13 Nov 2021 08:52:27 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 13 Nov 2021 08:52:28 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 13 Nov 2021 08:52:29 GMT
EXPOSE 3333
# Sat, 13 Nov 2021 08:52:31 GMT
COPY file:adf94c8c97044786e05e265ac7a3db4da2f14483f49d1d5b4e825de9c263b6f7 in /home/eggdrop/eggdrop 
# Sat, 13 Nov 2021 08:52:32 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 13 Nov 2021 08:52:32 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 13 Nov 2021 08:52:33 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:b48a9fe99aba73065302163e59c82a1b0054810c7b9ef85eee6f1b495b162461`  
		Last Modified: Fri, 12 Nov 2021 16:41:35 GMT  
		Size: 2.7 MB (2728748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5e043b67ff2353188b91df7f18b9d6303a74dfab8ddbb4db3728b472d64f8a`  
		Last Modified: Sat, 13 Nov 2021 11:11:50 GMT  
		Size: 1.2 KB (1235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0405e4fb852476c00df2b9492fe26cb8808a4289859d547bf3fa6d64c7bbad`  
		Last Modified: Sat, 13 Nov 2021 11:11:48 GMT  
		Size: 9.4 KB (9445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98322a765eb39902765567678e96d10de88f46f9b891d05f35d9bd23e82b0657`  
		Last Modified: Sat, 13 Nov 2021 11:11:48 GMT  
		Size: 2.7 MB (2721970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bdda7ca8a68c3ef9b15288227172a8bec3ad3c17a25bbae6c87a3b130b62a5`  
		Last Modified: Sat, 13 Nov 2021 11:11:49 GMT  
		Size: 8.5 MB (8469526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c09ac811e036ac0a4b650e3babedf24d7a9b7181704c67a3ba8e9c6603f39cc`  
		Last Modified: Sat, 13 Nov 2021 11:11:47 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54dea7d298717e7a3a2673a17ac32f21709df757929cf0e6a1254849b81b2cba`  
		Last Modified: Sat, 13 Nov 2021 11:11:47 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:latest`

```console
$ docker pull eggdrop@sha256:da791d7beb860dc9067745220f3f6d0437003c4fc7014b1256c367cf85405d48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:latest` - linux; amd64

```console
$ docker pull eggdrop@sha256:6e892a67931479b599c272a667e2938484206e52d7264ff14d7b7db016f37b30
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8289929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15447097e0374d1ea165db47231adde6fb63ff6480b16f30134b7a313a3b43e9`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:49:03 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 01 Sep 2021 00:49:05 GMT
RUN adduser -S eggdrop
# Wed, 01 Sep 2021 00:49:07 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 01 Sep 2021 00:49:10 GMT
RUN apk add --no-cache tcl bash openssl
# Wed, 01 Sep 2021 00:50:26 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.1.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.1.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.1.tar.gz.asc eggdrop-1.9.1.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.1.tar.gz.asc   && tar -zxvf eggdrop-1.9.1.tar.gz   && rm eggdrop-1.9.1.tar.gz   && ( cd eggdrop-1.9.1     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.1   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 01 Sep 2021 00:50:26 GMT
ENV NICK=
# Wed, 01 Sep 2021 00:50:27 GMT
ENV SERVER=
# Wed, 01 Sep 2021 00:50:27 GMT
ENV LISTEN=3333
# Wed, 01 Sep 2021 00:50:27 GMT
ENV OWNER=
# Wed, 01 Sep 2021 00:50:27 GMT
ENV USERFILE=eggdrop.user
# Wed, 01 Sep 2021 00:50:27 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 01 Sep 2021 00:50:28 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 01 Sep 2021 00:50:28 GMT
EXPOSE 3333
# Wed, 01 Sep 2021 00:50:28 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Wed, 01 Sep 2021 00:50:28 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 01 Sep 2021 00:50:29 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 01 Sep 2021 00:50:29 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2739640d4bb626124033590fe2bf187a76c1f09fc23aa7686e7c3fab1ea81d84`  
		Last Modified: Wed, 01 Sep 2021 00:51:19 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738ab5f4a6a9c53e0f6ed425003f94b60df8ec4e166993682419cfe0a94a62f5`  
		Last Modified: Wed, 01 Sep 2021 00:51:16 GMT  
		Size: 10.1 KB (10118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0880ee1cbcc03493b50e3d163c452ce2bbb7b3de40bf0f955c9744388500b821`  
		Last Modified: Wed, 01 Sep 2021 00:51:17 GMT  
		Size: 2.7 MB (2724823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734b1d2617820fb511e667242f74784e1a91e810da7643c518373cea683dc9f5`  
		Last Modified: Wed, 01 Sep 2021 00:51:17 GMT  
		Size: 2.7 MB (2737114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2384c732a6a65e03999103c3cb481f0e361b99732133b52e23f57be3a24759`  
		Last Modified: Wed, 01 Sep 2021 00:51:16 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4ab1d804e5474fe3998c40986e14f69650bea83115a3f78da3e35a49da8219`  
		Last Modified: Wed, 01 Sep 2021 00:51:16 GMT  
		Size: 698.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:latest` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:256bf1e8371ae1436bd7b27b318801ba886744ed2a1225293f5d586fac79f541
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7984703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c777347de3a39dff1a465be9c70eeda9ba5de814025ba8d418620d17956a5a7b`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Tue, 31 Aug 2021 22:30:33 GMT
ADD file:ed2b5e0fbd1e7ae37ab8f808c827d23c6841ce1edd7427552d5bf741d67ebcc0 in / 
# Tue, 31 Aug 2021 22:30:33 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 01:40:18 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 01 Sep 2021 01:40:20 GMT
RUN adduser -S eggdrop
# Wed, 01 Sep 2021 01:40:22 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 01 Sep 2021 01:40:25 GMT
RUN apk add --no-cache tcl bash openssl
# Wed, 01 Sep 2021 01:42:54 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.1.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.1.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.1.tar.gz.asc eggdrop-1.9.1.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.1.tar.gz.asc   && tar -zxvf eggdrop-1.9.1.tar.gz   && rm eggdrop-1.9.1.tar.gz   && ( cd eggdrop-1.9.1     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.1   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 01 Sep 2021 01:42:54 GMT
ENV NICK=
# Wed, 01 Sep 2021 01:42:55 GMT
ENV SERVER=
# Wed, 01 Sep 2021 01:42:55 GMT
ENV LISTEN=3333
# Wed, 01 Sep 2021 01:42:56 GMT
ENV OWNER=
# Wed, 01 Sep 2021 01:42:56 GMT
ENV USERFILE=eggdrop.user
# Wed, 01 Sep 2021 01:42:56 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 01 Sep 2021 01:42:57 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 01 Sep 2021 01:42:57 GMT
EXPOSE 3333
# Wed, 01 Sep 2021 01:42:58 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Wed, 01 Sep 2021 01:42:58 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 01 Sep 2021 01:42:59 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 01 Sep 2021 01:42:59 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:840d18d84f6afdc3231d126fdd3f84f23f0335b61cbfa9cb8808b888a4308919`  
		Last Modified: Tue, 31 Aug 2021 22:32:11 GMT  
		Size: 2.6 MB (2623761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f046c2415fb1127f8d46523c533c6d2cce3bd492e0d68c48c260d220336ca952`  
		Last Modified: Wed, 01 Sep 2021 01:43:59 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf336ff3aa2db3f62c40723c1adc70b28e83510d2314cff15dcb5e218e1c2af`  
		Last Modified: Wed, 01 Sep 2021 01:43:57 GMT  
		Size: 9.8 KB (9833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87713f793a04367c6610fc1476e6a6f31d2e474ebb4598fde28a9728dbd06ae`  
		Last Modified: Wed, 01 Sep 2021 01:43:59 GMT  
		Size: 2.7 MB (2652189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7192b1f59b63dc171f423af626fa69dc717358b1645dd0db5b1ed1fb3cbbb2bc`  
		Last Modified: Wed, 01 Sep 2021 01:43:59 GMT  
		Size: 2.7 MB (2695121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c74d83e6f19d90b93b685a87dd4c0c1b522bc2338d4fe8c56b9806a195ca45`  
		Last Modified: Wed, 01 Sep 2021 01:43:57 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6402fc12bd28bda7948b0b77e3a48bd0ebb3f7d2ce610b45949fcfc92e8e478a`  
		Last Modified: Wed, 01 Sep 2021 01:43:57 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:latest` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:bff7cdffd49712f662b1cde3d2375d386b65b1d3e7a9d91df91436e887bb32cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8210746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d1b5ae8312bcd75a3d6d7db1867b4f7070e3b7ed4e1ca97549a9e3c9f5d577f`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 15:15:36 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 01 Sep 2021 15:15:37 GMT
RUN adduser -S eggdrop
# Wed, 01 Sep 2021 15:15:38 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 01 Sep 2021 15:15:40 GMT
RUN apk add --no-cache tcl bash openssl
# Wed, 01 Sep 2021 15:16:52 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.1.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.1.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.1.tar.gz.asc eggdrop-1.9.1.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.1.tar.gz.asc   && tar -zxvf eggdrop-1.9.1.tar.gz   && rm eggdrop-1.9.1.tar.gz   && ( cd eggdrop-1.9.1     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.1   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 01 Sep 2021 15:16:52 GMT
ENV NICK=
# Wed, 01 Sep 2021 15:16:52 GMT
ENV SERVER=
# Wed, 01 Sep 2021 15:16:53 GMT
ENV LISTEN=3333
# Wed, 01 Sep 2021 15:16:53 GMT
ENV OWNER=
# Wed, 01 Sep 2021 15:16:53 GMT
ENV USERFILE=eggdrop.user
# Wed, 01 Sep 2021 15:16:53 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 01 Sep 2021 15:16:53 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 01 Sep 2021 15:16:53 GMT
EXPOSE 3333
# Wed, 01 Sep 2021 15:16:54 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Wed, 01 Sep 2021 15:16:54 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 01 Sep 2021 15:16:54 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 01 Sep 2021 15:16:54 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf67b3e836d0edeb34044ffda17873e401619019ce483f22005e430bc1433d4`  
		Last Modified: Wed, 01 Sep 2021 15:17:30 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b59c6abd4c336393a25dbe734281b04d79212c90032285294352d9d3f78958e`  
		Last Modified: Wed, 01 Sep 2021 15:17:28 GMT  
		Size: 10.0 KB (9995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae931fd0b19febff0674f2c50c3aa65d9c43ba202ee949c3de1aec49d6546c5e`  
		Last Modified: Wed, 01 Sep 2021 15:17:28 GMT  
		Size: 2.8 MB (2752469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5521e7d97fa85dd2c1c5040eedc8afdcd905ffddf8eae87dcdecc9d1a950b4e6`  
		Last Modified: Wed, 01 Sep 2021 15:17:28 GMT  
		Size: 2.7 MB (2731473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517861ca5ee30a5ce6da73542fdb0b2cbdfdf1bb73d813e0e39e8bdd9f0ce77e`  
		Last Modified: Wed, 01 Sep 2021 15:17:28 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2278cfa27b2d9e72ddec10cbe8092918ff164b9f10a6b6a0356017b49a94ba`  
		Last Modified: Wed, 01 Sep 2021 15:17:28 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:stable`

```console
$ docker pull eggdrop@sha256:da791d7beb860dc9067745220f3f6d0437003c4fc7014b1256c367cf85405d48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:stable` - linux; amd64

```console
$ docker pull eggdrop@sha256:6e892a67931479b599c272a667e2938484206e52d7264ff14d7b7db016f37b30
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8289929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15447097e0374d1ea165db47231adde6fb63ff6480b16f30134b7a313a3b43e9`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:49:03 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 01 Sep 2021 00:49:05 GMT
RUN adduser -S eggdrop
# Wed, 01 Sep 2021 00:49:07 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 01 Sep 2021 00:49:10 GMT
RUN apk add --no-cache tcl bash openssl
# Wed, 01 Sep 2021 00:50:26 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.1.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.1.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.1.tar.gz.asc eggdrop-1.9.1.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.1.tar.gz.asc   && tar -zxvf eggdrop-1.9.1.tar.gz   && rm eggdrop-1.9.1.tar.gz   && ( cd eggdrop-1.9.1     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.1   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 01 Sep 2021 00:50:26 GMT
ENV NICK=
# Wed, 01 Sep 2021 00:50:27 GMT
ENV SERVER=
# Wed, 01 Sep 2021 00:50:27 GMT
ENV LISTEN=3333
# Wed, 01 Sep 2021 00:50:27 GMT
ENV OWNER=
# Wed, 01 Sep 2021 00:50:27 GMT
ENV USERFILE=eggdrop.user
# Wed, 01 Sep 2021 00:50:27 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 01 Sep 2021 00:50:28 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 01 Sep 2021 00:50:28 GMT
EXPOSE 3333
# Wed, 01 Sep 2021 00:50:28 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Wed, 01 Sep 2021 00:50:28 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 01 Sep 2021 00:50:29 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 01 Sep 2021 00:50:29 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2739640d4bb626124033590fe2bf187a76c1f09fc23aa7686e7c3fab1ea81d84`  
		Last Modified: Wed, 01 Sep 2021 00:51:19 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738ab5f4a6a9c53e0f6ed425003f94b60df8ec4e166993682419cfe0a94a62f5`  
		Last Modified: Wed, 01 Sep 2021 00:51:16 GMT  
		Size: 10.1 KB (10118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0880ee1cbcc03493b50e3d163c452ce2bbb7b3de40bf0f955c9744388500b821`  
		Last Modified: Wed, 01 Sep 2021 00:51:17 GMT  
		Size: 2.7 MB (2724823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734b1d2617820fb511e667242f74784e1a91e810da7643c518373cea683dc9f5`  
		Last Modified: Wed, 01 Sep 2021 00:51:17 GMT  
		Size: 2.7 MB (2737114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2384c732a6a65e03999103c3cb481f0e361b99732133b52e23f57be3a24759`  
		Last Modified: Wed, 01 Sep 2021 00:51:16 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4ab1d804e5474fe3998c40986e14f69650bea83115a3f78da3e35a49da8219`  
		Last Modified: Wed, 01 Sep 2021 00:51:16 GMT  
		Size: 698.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:stable` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:256bf1e8371ae1436bd7b27b318801ba886744ed2a1225293f5d586fac79f541
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7984703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c777347de3a39dff1a465be9c70eeda9ba5de814025ba8d418620d17956a5a7b`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Tue, 31 Aug 2021 22:30:33 GMT
ADD file:ed2b5e0fbd1e7ae37ab8f808c827d23c6841ce1edd7427552d5bf741d67ebcc0 in / 
# Tue, 31 Aug 2021 22:30:33 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 01:40:18 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 01 Sep 2021 01:40:20 GMT
RUN adduser -S eggdrop
# Wed, 01 Sep 2021 01:40:22 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 01 Sep 2021 01:40:25 GMT
RUN apk add --no-cache tcl bash openssl
# Wed, 01 Sep 2021 01:42:54 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.1.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.1.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.1.tar.gz.asc eggdrop-1.9.1.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.1.tar.gz.asc   && tar -zxvf eggdrop-1.9.1.tar.gz   && rm eggdrop-1.9.1.tar.gz   && ( cd eggdrop-1.9.1     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.1   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 01 Sep 2021 01:42:54 GMT
ENV NICK=
# Wed, 01 Sep 2021 01:42:55 GMT
ENV SERVER=
# Wed, 01 Sep 2021 01:42:55 GMT
ENV LISTEN=3333
# Wed, 01 Sep 2021 01:42:56 GMT
ENV OWNER=
# Wed, 01 Sep 2021 01:42:56 GMT
ENV USERFILE=eggdrop.user
# Wed, 01 Sep 2021 01:42:56 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 01 Sep 2021 01:42:57 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 01 Sep 2021 01:42:57 GMT
EXPOSE 3333
# Wed, 01 Sep 2021 01:42:58 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Wed, 01 Sep 2021 01:42:58 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 01 Sep 2021 01:42:59 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 01 Sep 2021 01:42:59 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:840d18d84f6afdc3231d126fdd3f84f23f0335b61cbfa9cb8808b888a4308919`  
		Last Modified: Tue, 31 Aug 2021 22:32:11 GMT  
		Size: 2.6 MB (2623761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f046c2415fb1127f8d46523c533c6d2cce3bd492e0d68c48c260d220336ca952`  
		Last Modified: Wed, 01 Sep 2021 01:43:59 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf336ff3aa2db3f62c40723c1adc70b28e83510d2314cff15dcb5e218e1c2af`  
		Last Modified: Wed, 01 Sep 2021 01:43:57 GMT  
		Size: 9.8 KB (9833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87713f793a04367c6610fc1476e6a6f31d2e474ebb4598fde28a9728dbd06ae`  
		Last Modified: Wed, 01 Sep 2021 01:43:59 GMT  
		Size: 2.7 MB (2652189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7192b1f59b63dc171f423af626fa69dc717358b1645dd0db5b1ed1fb3cbbb2bc`  
		Last Modified: Wed, 01 Sep 2021 01:43:59 GMT  
		Size: 2.7 MB (2695121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c74d83e6f19d90b93b685a87dd4c0c1b522bc2338d4fe8c56b9806a195ca45`  
		Last Modified: Wed, 01 Sep 2021 01:43:57 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6402fc12bd28bda7948b0b77e3a48bd0ebb3f7d2ce610b45949fcfc92e8e478a`  
		Last Modified: Wed, 01 Sep 2021 01:43:57 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:stable` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:bff7cdffd49712f662b1cde3d2375d386b65b1d3e7a9d91df91436e887bb32cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8210746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d1b5ae8312bcd75a3d6d7db1867b4f7070e3b7ed4e1ca97549a9e3c9f5d577f`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 15:15:36 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 01 Sep 2021 15:15:37 GMT
RUN adduser -S eggdrop
# Wed, 01 Sep 2021 15:15:38 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 01 Sep 2021 15:15:40 GMT
RUN apk add --no-cache tcl bash openssl
# Wed, 01 Sep 2021 15:16:52 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.1.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.1.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.1.tar.gz.asc eggdrop-1.9.1.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.1.tar.gz.asc   && tar -zxvf eggdrop-1.9.1.tar.gz   && rm eggdrop-1.9.1.tar.gz   && ( cd eggdrop-1.9.1     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.1   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 01 Sep 2021 15:16:52 GMT
ENV NICK=
# Wed, 01 Sep 2021 15:16:52 GMT
ENV SERVER=
# Wed, 01 Sep 2021 15:16:53 GMT
ENV LISTEN=3333
# Wed, 01 Sep 2021 15:16:53 GMT
ENV OWNER=
# Wed, 01 Sep 2021 15:16:53 GMT
ENV USERFILE=eggdrop.user
# Wed, 01 Sep 2021 15:16:53 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 01 Sep 2021 15:16:53 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 01 Sep 2021 15:16:53 GMT
EXPOSE 3333
# Wed, 01 Sep 2021 15:16:54 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Wed, 01 Sep 2021 15:16:54 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 01 Sep 2021 15:16:54 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 01 Sep 2021 15:16:54 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf67b3e836d0edeb34044ffda17873e401619019ce483f22005e430bc1433d4`  
		Last Modified: Wed, 01 Sep 2021 15:17:30 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b59c6abd4c336393a25dbe734281b04d79212c90032285294352d9d3f78958e`  
		Last Modified: Wed, 01 Sep 2021 15:17:28 GMT  
		Size: 10.0 KB (9995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae931fd0b19febff0674f2c50c3aa65d9c43ba202ee949c3de1aec49d6546c5e`  
		Last Modified: Wed, 01 Sep 2021 15:17:28 GMT  
		Size: 2.8 MB (2752469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5521e7d97fa85dd2c1c5040eedc8afdcd905ffddf8eae87dcdecc9d1a950b4e6`  
		Last Modified: Wed, 01 Sep 2021 15:17:28 GMT  
		Size: 2.7 MB (2731473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517861ca5ee30a5ce6da73542fdb0b2cbdfdf1bb73d813e0e39e8bdd9f0ce77e`  
		Last Modified: Wed, 01 Sep 2021 15:17:28 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2278cfa27b2d9e72ddec10cbe8092918ff164b9f10a6b6a0356017b49a94ba`  
		Last Modified: Wed, 01 Sep 2021 15:17:28 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
