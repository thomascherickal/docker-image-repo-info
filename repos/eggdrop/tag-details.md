<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `eggdrop`

-	[`eggdrop:1.9`](#eggdrop19)
-	[`eggdrop:1.9.5`](#eggdrop195)
-	[`eggdrop:develop`](#eggdropdevelop)
-	[`eggdrop:latest`](#eggdroplatest)
-	[`eggdrop:stable`](#eggdropstable)

## `eggdrop:1.9`

```console
$ docker pull eggdrop@sha256:ec2179041ce79ebd4fab44616ade6ef5eacbcc1ab3e4348990aa48b0257d7bf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:1.9` - linux; amd64

```console
$ docker pull eggdrop@sha256:7d503e0bbbcf926621597e8442d5b75273ed5f51cbaebf5ca4c32e1cbca62d6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.7 MB (11707730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94885e42bceb6f392a87abdba804b2649c33d961d93aaa1cfd4ae23b75cdacdf`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:51:45 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 11 Feb 2023 07:51:46 GMT
RUN adduser -S eggdrop
# Sat, 11 Feb 2023 07:51:46 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 11 Feb 2023 07:51:48 GMT
RUN apk add --no-cache tcl bash openssl
# Sat, 11 Feb 2023 07:55:46 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.4.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.4.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.4.tar.gz.asc eggdrop-1.9.4.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.4.tar.gz.asc   && tar -zxvf eggdrop-1.9.4.tar.gz   && rm eggdrop-1.9.4.tar.gz   && ( cd eggdrop-1.9.4     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.4   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 11 Feb 2023 07:55:46 GMT
ENV NICK=
# Sat, 11 Feb 2023 07:55:46 GMT
ENV SERVER=
# Sat, 11 Feb 2023 07:55:47 GMT
ENV LISTEN=3333
# Sat, 11 Feb 2023 07:55:47 GMT
ENV OWNER=
# Sat, 11 Feb 2023 07:55:47 GMT
ENV USERFILE=eggdrop.user
# Sat, 11 Feb 2023 07:55:47 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 11 Feb 2023 07:55:47 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 11 Feb 2023 07:55:47 GMT
EXPOSE 3333
# Sat, 11 Feb 2023 07:55:47 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Sat, 11 Feb 2023 07:55:47 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 11 Feb 2023 07:55:47 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 11 Feb 2023 07:55:48 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5929d6c17ae9e3c1785e747f2e1c9a4043d1271b0b4fa46fd3b5d69e688807c3`  
		Last Modified: Sat, 11 Feb 2023 07:56:10 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45534f8d250972e326ebb489c727bd241fe3ff4b1127eb39d1d672b0168cca9e`  
		Last Modified: Sat, 11 Feb 2023 07:56:08 GMT  
		Size: 10.9 KB (10932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c10f44dd07312e4c61cf11012690bfbb08c68a17c2cbd5e4c5bec99e2dcecf`  
		Last Modified: Sat, 11 Feb 2023 07:56:09 GMT  
		Size: 2.8 MB (2757983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da126ee1240a822d73b85fe7646d08199ddab22146b346b6082d64822089bbfa`  
		Last Modified: Sat, 11 Feb 2023 07:56:09 GMT  
		Size: 6.1 MB (6127248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d97460e3eba8e8c667065808ae8282c0b7ddf147ddae13b3a5553a431bcccdd0`  
		Last Modified: Sat, 11 Feb 2023 07:56:08 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f385e4dbc86989aa993e14712f5523b1dd3458d9c4b311d202765f34873e60`  
		Last Modified: Sat, 11 Feb 2023 07:56:08 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:1.9` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:add1154fcd484e80e959a680b538c3bfd2a25aedc5e2db342f32572170880ef0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.4 MB (11352013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4da83a66d4ecc8fc4b5598adbac4cd7c21311a640733c0db906a4b0b9a6a8dba`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:48 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Mon, 13 Mar 2023 16:12:48 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 17:12:15 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Mon, 13 Mar 2023 17:12:16 GMT
RUN adduser -S eggdrop
# Mon, 13 Mar 2023 17:12:17 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 13 Mar 2023 17:12:19 GMT
RUN apk add --no-cache tcl bash openssl
# Mon, 13 Mar 2023 17:16:35 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.4.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.4.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.4.tar.gz.asc eggdrop-1.9.4.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.4.tar.gz.asc   && tar -zxvf eggdrop-1.9.4.tar.gz   && rm eggdrop-1.9.4.tar.gz   && ( cd eggdrop-1.9.4     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.4   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 13 Mar 2023 17:16:35 GMT
ENV NICK=
# Mon, 13 Mar 2023 17:16:35 GMT
ENV SERVER=
# Mon, 13 Mar 2023 17:16:35 GMT
ENV LISTEN=3333
# Mon, 13 Mar 2023 17:16:36 GMT
ENV OWNER=
# Mon, 13 Mar 2023 17:16:36 GMT
ENV USERFILE=eggdrop.user
# Mon, 13 Mar 2023 17:16:36 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 13 Mar 2023 17:16:36 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 13 Mar 2023 17:16:36 GMT
EXPOSE 3333
# Mon, 13 Mar 2023 17:16:36 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Mon, 13 Mar 2023 17:16:36 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 13 Mar 2023 17:16:36 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 13 Mar 2023 17:16:36 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ec2417a5f95cb8476bdb0bd490a3653224f7fbdf8ed2d8ad59f0de673e0d67`  
		Last Modified: Mon, 13 Mar 2023 17:17:05 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f559d903a28746e7b2cf18297c1dbd3ed8df78227b31a55764027bb8c88190`  
		Last Modified: Mon, 13 Mar 2023 17:17:03 GMT  
		Size: 10.6 KB (10638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f4bd0129aa84d8df20f9b5ed48a4a123ec3cc83121d834bc9e5e55e32a2373`  
		Last Modified: Mon, 13 Mar 2023 17:17:04 GMT  
		Size: 2.7 MB (2679912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca42b7876bf72171c45ac71c6d89f12218cc82ee2bea7227ea98efef4b97d22`  
		Last Modified: Mon, 13 Mar 2023 17:17:05 GMT  
		Size: 6.0 MB (6040868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e353d64f03127a8631c30ac73e868b707101a590d5b35332915ce50036835c`  
		Last Modified: Mon, 13 Mar 2023 17:17:03 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9ed6c536151b03b35d7e2c5575691fc2f72693d3d8ad65af13ab3414df0490`  
		Last Modified: Mon, 13 Mar 2023 17:17:03 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:1.9` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:0abf618712457a362bea4768e49625dfbcb932423fb8ff4d3e48820c05eab23b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.7 MB (11687675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d3649ae583cdf8dd6866df445c5c9372471e97e2191dc50c7e96a97a2247094`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:14:57 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Fri, 10 Feb 2023 22:14:58 GMT
RUN adduser -S eggdrop
# Fri, 10 Feb 2023 22:14:59 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Fri, 10 Feb 2023 22:15:00 GMT
RUN apk add --no-cache tcl bash openssl
# Mon, 13 Mar 2023 19:46:33 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.5.tar.gz.asc eggdrop-1.9.5.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.5.tar.gz.asc   && tar -zxvf eggdrop-1.9.5.tar.gz   && rm eggdrop-1.9.5.tar.gz   && ( cd eggdrop-1.9.5     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.5   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 13 Mar 2023 19:46:33 GMT
ENV NICK=
# Mon, 13 Mar 2023 19:46:33 GMT
ENV SERVER=
# Mon, 13 Mar 2023 19:46:33 GMT
ENV LISTEN=3333
# Mon, 13 Mar 2023 19:46:33 GMT
ENV OWNER=
# Mon, 13 Mar 2023 19:46:33 GMT
ENV USERFILE=eggdrop.user
# Mon, 13 Mar 2023 19:46:33 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 13 Mar 2023 19:46:33 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 13 Mar 2023 19:46:34 GMT
EXPOSE 3333
# Mon, 13 Mar 2023 19:46:34 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Mon, 13 Mar 2023 19:46:34 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 13 Mar 2023 19:46:34 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 13 Mar 2023 19:46:34 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddb182a5cc1394eccbeeef59c5ad5d259ed5ddd4cdd2a1d4c5ad107256b7a2ee`  
		Last Modified: Fri, 10 Feb 2023 22:19:08 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59923206b30ea4054c1bb753aa8a5404a199d12f865dc365b1f8eb66fdb817b`  
		Last Modified: Fri, 10 Feb 2023 22:19:06 GMT  
		Size: 10.7 KB (10747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78dd68e4187ad121351dbe2536603e4802110332e9e21ecccff44b92d2ea68b5`  
		Last Modified: Fri, 10 Feb 2023 22:19:07 GMT  
		Size: 2.8 MB (2776467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0ddce20c0ea549cec6107f845beb13933ad23e830831793e93aa9608201939`  
		Last Modified: Mon, 13 Mar 2023 19:47:02 GMT  
		Size: 6.2 MB (6187136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93516d805e7d87b11e0b6272b3ad0d97e326a54cfc193b65a1f78193a2b105f`  
		Last Modified: Mon, 13 Mar 2023 19:47:01 GMT  
		Size: 1.8 KB (1844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00748ce261013a78b5d9d65606290d1ad4820d004dde3489c9e960d0a62846b2`  
		Last Modified: Mon, 13 Mar 2023 19:47:01 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:1.9.5`

```console
$ docker pull eggdrop@sha256:a6f2b6a9f3507afe6723caabe5d466baafcec76b01181f7938ca91575b8fa699
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `eggdrop:1.9.5` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:0abf618712457a362bea4768e49625dfbcb932423fb8ff4d3e48820c05eab23b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.7 MB (11687675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d3649ae583cdf8dd6866df445c5c9372471e97e2191dc50c7e96a97a2247094`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:14:57 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Fri, 10 Feb 2023 22:14:58 GMT
RUN adduser -S eggdrop
# Fri, 10 Feb 2023 22:14:59 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Fri, 10 Feb 2023 22:15:00 GMT
RUN apk add --no-cache tcl bash openssl
# Mon, 13 Mar 2023 19:46:33 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.5.tar.gz.asc eggdrop-1.9.5.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.5.tar.gz.asc   && tar -zxvf eggdrop-1.9.5.tar.gz   && rm eggdrop-1.9.5.tar.gz   && ( cd eggdrop-1.9.5     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.5   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 13 Mar 2023 19:46:33 GMT
ENV NICK=
# Mon, 13 Mar 2023 19:46:33 GMT
ENV SERVER=
# Mon, 13 Mar 2023 19:46:33 GMT
ENV LISTEN=3333
# Mon, 13 Mar 2023 19:46:33 GMT
ENV OWNER=
# Mon, 13 Mar 2023 19:46:33 GMT
ENV USERFILE=eggdrop.user
# Mon, 13 Mar 2023 19:46:33 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 13 Mar 2023 19:46:33 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 13 Mar 2023 19:46:34 GMT
EXPOSE 3333
# Mon, 13 Mar 2023 19:46:34 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Mon, 13 Mar 2023 19:46:34 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 13 Mar 2023 19:46:34 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 13 Mar 2023 19:46:34 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddb182a5cc1394eccbeeef59c5ad5d259ed5ddd4cdd2a1d4c5ad107256b7a2ee`  
		Last Modified: Fri, 10 Feb 2023 22:19:08 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59923206b30ea4054c1bb753aa8a5404a199d12f865dc365b1f8eb66fdb817b`  
		Last Modified: Fri, 10 Feb 2023 22:19:06 GMT  
		Size: 10.7 KB (10747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78dd68e4187ad121351dbe2536603e4802110332e9e21ecccff44b92d2ea68b5`  
		Last Modified: Fri, 10 Feb 2023 22:19:07 GMT  
		Size: 2.8 MB (2776467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0ddce20c0ea549cec6107f845beb13933ad23e830831793e93aa9608201939`  
		Last Modified: Mon, 13 Mar 2023 19:47:02 GMT  
		Size: 6.2 MB (6187136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93516d805e7d87b11e0b6272b3ad0d97e326a54cfc193b65a1f78193a2b105f`  
		Last Modified: Mon, 13 Mar 2023 19:47:01 GMT  
		Size: 1.8 KB (1844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00748ce261013a78b5d9d65606290d1ad4820d004dde3489c9e960d0a62846b2`  
		Last Modified: Mon, 13 Mar 2023 19:47:01 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:develop`

```console
$ docker pull eggdrop@sha256:89c1c21e469cbf5ad08e17e86d47f802d304ce735ce440ffa377e97b88f6b1bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:develop` - linux; amd64

```console
$ docker pull eggdrop@sha256:86b82bcbc18e3d56b832d60f0f242f07ea8131f12df1273232d23be7f5298ceb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14619050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:289b31aa30810d9f17fb7629fa43c6be80532051b8daddb882ccf7b2f91eb278`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:54 GMT
ADD file:cdac18271416ac5bf6876b7ea9af1129108d03f9813589dfda113e5f09d6b80b in / 
# Sat, 11 Feb 2023 04:46:55 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:47:36 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 11 Feb 2023 07:47:37 GMT
RUN adduser -S eggdrop
# Sat, 11 Feb 2023 07:47:38 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 11 Feb 2023 07:47:38 GMT
ENV EGGDROP_SHA256=caafc1ad001e2e77793dca37998cb94d88efadb4ec9c3de44c1004b04f15aa6e
# Sat, 11 Feb 2023 07:47:38 GMT
ENV EGGDROP_COMMIT=2a6a36888f5aa2204d84a9e6282d35e5421c2c8a
# Sat, 11 Feb 2023 07:47:39 GMT
RUN apk --update add --no-cache bash openssl
# Sat, 11 Feb 2023 07:51:31 GMT
RUN apk --update add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.13-src.tar.gz" -O tcl8.6.13-src.tar.gz   && tar -zxf tcl8.6.13-src.tar.gz   && ( cd tcl8.6.13     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm -rf tcl8.6.13-src.tar.gz   && rm -rf tcl8.6.13   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 11 Feb 2023 07:51:31 GMT
ENV NICK=
# Sat, 11 Feb 2023 07:51:31 GMT
ENV SERVER=
# Sat, 11 Feb 2023 07:51:31 GMT
ENV LISTEN=3333
# Sat, 11 Feb 2023 07:51:31 GMT
ENV OWNER=
# Sat, 11 Feb 2023 07:51:31 GMT
ENV USERFILE=eggdrop.user
# Sat, 11 Feb 2023 07:51:32 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 11 Feb 2023 07:51:32 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 11 Feb 2023 07:51:32 GMT
EXPOSE 3333
# Sat, 11 Feb 2023 07:51:32 GMT
COPY file:35e05bb72116a1848ec779e3fbc4ea6bbcd95ceb11059751f608c8543e18cde7 in /home/eggdrop/eggdrop 
# Sat, 11 Feb 2023 07:51:32 GMT
COPY file:f30bcb89ff6df7709069d6cc97353d72cdbbebc6530d8d350cbb3ae4dad79129 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 11 Feb 2023 07:51:32 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 11 Feb 2023 07:51:32 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:895e193edb5191bf66fb5ccb29f5d3659e05eec5953255180cbdd66520e7c517`  
		Last Modified: Sat, 11 Feb 2023 04:47:40 GMT  
		Size: 2.8 MB (2826146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40b4bba832da1fec1519d1be2d63ef0ffcc84d75b6db6df42c4c59d6bc7909f`  
		Last Modified: Sat, 11 Feb 2023 07:56:03 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc75a393c23b0e781af338ef981ff56ba6433c3207c9600ecfb5b0b5ef0b07b`  
		Last Modified: Sat, 11 Feb 2023 07:56:01 GMT  
		Size: 11.0 KB (10959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334aa6104162d045953c318a6a719bc3a96f1408bf6f8304b3daa2459e6a3f4b`  
		Last Modified: Sat, 11 Feb 2023 07:56:01 GMT  
		Size: 1.1 MB (1090108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ae2f8ea1a1ec72a7be9dfaf03a2b60e708c62bfc43330786b4b9611f2403ef`  
		Last Modified: Sat, 11 Feb 2023 07:56:03 GMT  
		Size: 10.7 MB (10687615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e861280f19c09b89f8a6cee053d730d9a6160de434bb76ff6a834729b1020c0`  
		Last Modified: Sat, 11 Feb 2023 07:56:01 GMT  
		Size: 1.9 KB (1891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e6216bb55278efc253dfc07f10d507274448cd217b1fc1d093a50e98089c15`  
		Last Modified: Sat, 11 Feb 2023 07:56:01 GMT  
		Size: 1.1 KB (1061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:6c86b6047dc17b5fa293f22c505ccb707fbc730c9ab919a035cd275ce8ea02b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14600188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be579805f3b42b833d668e6808cc1d31b6a3b83b76060aaf4b7a2dbfb839f60f`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:51 GMT
ADD file:141468a99f598ddb90dbb73978d10c0f00d01ece185e157ac33a0a1414d45944 in / 
# Mon, 13 Mar 2023 16:12:51 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 17:07:36 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Mon, 13 Mar 2023 17:07:36 GMT
RUN adduser -S eggdrop
# Mon, 13 Mar 2023 17:07:37 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 13 Mar 2023 17:07:37 GMT
ENV EGGDROP_SHA256=caafc1ad001e2e77793dca37998cb94d88efadb4ec9c3de44c1004b04f15aa6e
# Mon, 13 Mar 2023 17:07:38 GMT
ENV EGGDROP_COMMIT=2a6a36888f5aa2204d84a9e6282d35e5421c2c8a
# Mon, 13 Mar 2023 17:07:38 GMT
RUN apk --update add --no-cache bash openssl
# Mon, 13 Mar 2023 17:12:02 GMT
RUN apk --update add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.13-src.tar.gz" -O tcl8.6.13-src.tar.gz   && tar -zxf tcl8.6.13-src.tar.gz   && ( cd tcl8.6.13     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm -rf tcl8.6.13-src.tar.gz   && rm -rf tcl8.6.13   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 13 Mar 2023 17:12:02 GMT
ENV NICK=
# Mon, 13 Mar 2023 17:12:03 GMT
ENV SERVER=
# Mon, 13 Mar 2023 17:12:03 GMT
ENV LISTEN=3333
# Mon, 13 Mar 2023 17:12:03 GMT
ENV OWNER=
# Mon, 13 Mar 2023 17:12:03 GMT
ENV USERFILE=eggdrop.user
# Mon, 13 Mar 2023 17:12:03 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 13 Mar 2023 17:12:03 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 13 Mar 2023 17:12:03 GMT
EXPOSE 3333
# Mon, 13 Mar 2023 17:12:03 GMT
COPY file:35e05bb72116a1848ec779e3fbc4ea6bbcd95ceb11059751f608c8543e18cde7 in /home/eggdrop/eggdrop 
# Mon, 13 Mar 2023 17:12:03 GMT
COPY file:f30bcb89ff6df7709069d6cc97353d72cdbbebc6530d8d350cbb3ae4dad79129 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 13 Mar 2023 17:12:03 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 13 Mar 2023 17:12:03 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:ed6cbaa656dcebfe8d252792a339ccf10dddd695875f07c9636d59a5baf85f3f`  
		Last Modified: Fri, 10 Feb 2023 20:50:51 GMT  
		Size: 2.6 MB (2633649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537e8916b76bf343b1c25f24dee977b9ba00d42451454c14399a30a7f370e44f`  
		Last Modified: Mon, 13 Mar 2023 17:16:56 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e00d23c139fb736958dc43befabbf8245ddd222d1886ebfe766aa6b20a8d7dc`  
		Last Modified: Mon, 13 Mar 2023 17:16:54 GMT  
		Size: 10.7 KB (10665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb3e9765bc71d5a74b4672a53c0fa391137f2514d6e52a557737e660148dca9`  
		Last Modified: Mon, 13 Mar 2023 17:16:55 GMT  
		Size: 1.0 MB (1032718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96a591dcf05a5f31cc5f1c68d9325a94c2f5f2651e100df4ad12a630d91d540`  
		Last Modified: Mon, 13 Mar 2023 17:16:56 GMT  
		Size: 10.9 MB (10918925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ea78a0466299eb626abd0283dfa101d053e6a8d4a27685fe3ccb7fbe5f0e40`  
		Last Modified: Mon, 13 Mar 2023 17:16:54 GMT  
		Size: 1.9 KB (1896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83379c51c0d2e1b6c6ac39c6ae65b3d38b0f8bff96f5d6defcc8a8a549c61282`  
		Last Modified: Mon, 13 Mar 2023 17:16:54 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:8516d995663b2cf5910f0507c9fd41dc7db01fa21efe289edabeb0e76f4614fd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16105068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a7bb92b403f21977cc7904a9adbc47062d6f3e7e6638f9bae0626de4e44016c`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 19:39:28 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Mon, 13 Mar 2023 19:39:28 GMT
RUN adduser -S eggdrop
# Mon, 13 Mar 2023 19:39:29 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 13 Mar 2023 19:39:29 GMT
ENV EGGDROP_SHA256=cc7936ee427959081651319119ac0b8f3581a18d7be7b20f71023954f1f69a91
# Mon, 13 Mar 2023 19:39:29 GMT
ENV EGGDROP_COMMIT=26ecf0921ee84c5bf61cb31014a75f02670b1af4
# Mon, 13 Mar 2023 19:39:30 GMT
RUN apk --update add --no-cache bash openssl
# Mon, 13 Mar 2023 19:42:44 GMT
RUN apk --update add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.13-src.tar.gz" -O tcl8.6.13-src.tar.gz   && tar -zxf tcl8.6.13-src.tar.gz   && ( cd tcl8.6.13     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm -rf tcl8.6.13-src.tar.gz   && rm -rf tcl8.6.13   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 13 Mar 2023 19:42:44 GMT
ENV NICK=
# Mon, 13 Mar 2023 19:42:44 GMT
ENV SERVER=
# Mon, 13 Mar 2023 19:42:44 GMT
ENV LISTEN=3333
# Mon, 13 Mar 2023 19:42:44 GMT
ENV OWNER=
# Mon, 13 Mar 2023 19:42:45 GMT
ENV USERFILE=eggdrop.user
# Mon, 13 Mar 2023 19:42:45 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 13 Mar 2023 19:42:45 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 13 Mar 2023 19:42:45 GMT
EXPOSE 3333
# Mon, 13 Mar 2023 19:42:45 GMT
COPY file:35e05bb72116a1848ec779e3fbc4ea6bbcd95ceb11059751f608c8543e18cde7 in /home/eggdrop/eggdrop 
# Mon, 13 Mar 2023 19:42:45 GMT
COPY file:f30bcb89ff6df7709069d6cc97353d72cdbbebc6530d8d350cbb3ae4dad79129 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 13 Mar 2023 19:42:45 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 13 Mar 2023 19:42:45 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027d7fd862438b5a7eab063f319483086590e99117b1ca23b99dd8ae685cf42a`  
		Last Modified: Mon, 13 Mar 2023 19:46:53 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3145396ffd838a69d8eac490e1a2c789871c608378afbcf8c3df40d8ab36f7e`  
		Last Modified: Mon, 13 Mar 2023 19:46:52 GMT  
		Size: 11.2 KB (11189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b194e27c5f4b901e34cfa9e151ead8fc0482b807e4f337ab5c5f9d74492436`  
		Last Modified: Mon, 13 Mar 2023 19:46:52 GMT  
		Size: 1.2 MB (1233188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9600e6d70d7dfab265638f1033d8daa6f3b39b1ea469c354e083d5efde6ad376`  
		Last Modified: Mon, 13 Mar 2023 19:46:53 GMT  
		Size: 11.6 MB (11594498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6836f32e6d90c561f6767490e4084eef1c0eaee8de9c6447cea44d0d5f7d4bef`  
		Last Modified: Mon, 13 Mar 2023 19:46:52 GMT  
		Size: 1.9 KB (1895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c8eb5985f3ca8d6db4ef154ddac10bfaa594d50252b32d48f313d5da7a66361`  
		Last Modified: Mon, 13 Mar 2023 19:46:52 GMT  
		Size: 1.1 KB (1064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:latest`

```console
$ docker pull eggdrop@sha256:ec2179041ce79ebd4fab44616ade6ef5eacbcc1ab3e4348990aa48b0257d7bf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:latest` - linux; amd64

```console
$ docker pull eggdrop@sha256:7d503e0bbbcf926621597e8442d5b75273ed5f51cbaebf5ca4c32e1cbca62d6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.7 MB (11707730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94885e42bceb6f392a87abdba804b2649c33d961d93aaa1cfd4ae23b75cdacdf`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:51:45 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 11 Feb 2023 07:51:46 GMT
RUN adduser -S eggdrop
# Sat, 11 Feb 2023 07:51:46 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 11 Feb 2023 07:51:48 GMT
RUN apk add --no-cache tcl bash openssl
# Sat, 11 Feb 2023 07:55:46 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.4.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.4.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.4.tar.gz.asc eggdrop-1.9.4.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.4.tar.gz.asc   && tar -zxvf eggdrop-1.9.4.tar.gz   && rm eggdrop-1.9.4.tar.gz   && ( cd eggdrop-1.9.4     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.4   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 11 Feb 2023 07:55:46 GMT
ENV NICK=
# Sat, 11 Feb 2023 07:55:46 GMT
ENV SERVER=
# Sat, 11 Feb 2023 07:55:47 GMT
ENV LISTEN=3333
# Sat, 11 Feb 2023 07:55:47 GMT
ENV OWNER=
# Sat, 11 Feb 2023 07:55:47 GMT
ENV USERFILE=eggdrop.user
# Sat, 11 Feb 2023 07:55:47 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 11 Feb 2023 07:55:47 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 11 Feb 2023 07:55:47 GMT
EXPOSE 3333
# Sat, 11 Feb 2023 07:55:47 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Sat, 11 Feb 2023 07:55:47 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 11 Feb 2023 07:55:47 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 11 Feb 2023 07:55:48 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5929d6c17ae9e3c1785e747f2e1c9a4043d1271b0b4fa46fd3b5d69e688807c3`  
		Last Modified: Sat, 11 Feb 2023 07:56:10 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45534f8d250972e326ebb489c727bd241fe3ff4b1127eb39d1d672b0168cca9e`  
		Last Modified: Sat, 11 Feb 2023 07:56:08 GMT  
		Size: 10.9 KB (10932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c10f44dd07312e4c61cf11012690bfbb08c68a17c2cbd5e4c5bec99e2dcecf`  
		Last Modified: Sat, 11 Feb 2023 07:56:09 GMT  
		Size: 2.8 MB (2757983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da126ee1240a822d73b85fe7646d08199ddab22146b346b6082d64822089bbfa`  
		Last Modified: Sat, 11 Feb 2023 07:56:09 GMT  
		Size: 6.1 MB (6127248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d97460e3eba8e8c667065808ae8282c0b7ddf147ddae13b3a5553a431bcccdd0`  
		Last Modified: Sat, 11 Feb 2023 07:56:08 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f385e4dbc86989aa993e14712f5523b1dd3458d9c4b311d202765f34873e60`  
		Last Modified: Sat, 11 Feb 2023 07:56:08 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:latest` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:add1154fcd484e80e959a680b538c3bfd2a25aedc5e2db342f32572170880ef0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.4 MB (11352013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4da83a66d4ecc8fc4b5598adbac4cd7c21311a640733c0db906a4b0b9a6a8dba`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:48 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Mon, 13 Mar 2023 16:12:48 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 17:12:15 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Mon, 13 Mar 2023 17:12:16 GMT
RUN adduser -S eggdrop
# Mon, 13 Mar 2023 17:12:17 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 13 Mar 2023 17:12:19 GMT
RUN apk add --no-cache tcl bash openssl
# Mon, 13 Mar 2023 17:16:35 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.4.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.4.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.4.tar.gz.asc eggdrop-1.9.4.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.4.tar.gz.asc   && tar -zxvf eggdrop-1.9.4.tar.gz   && rm eggdrop-1.9.4.tar.gz   && ( cd eggdrop-1.9.4     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.4   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 13 Mar 2023 17:16:35 GMT
ENV NICK=
# Mon, 13 Mar 2023 17:16:35 GMT
ENV SERVER=
# Mon, 13 Mar 2023 17:16:35 GMT
ENV LISTEN=3333
# Mon, 13 Mar 2023 17:16:36 GMT
ENV OWNER=
# Mon, 13 Mar 2023 17:16:36 GMT
ENV USERFILE=eggdrop.user
# Mon, 13 Mar 2023 17:16:36 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 13 Mar 2023 17:16:36 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 13 Mar 2023 17:16:36 GMT
EXPOSE 3333
# Mon, 13 Mar 2023 17:16:36 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Mon, 13 Mar 2023 17:16:36 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 13 Mar 2023 17:16:36 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 13 Mar 2023 17:16:36 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ec2417a5f95cb8476bdb0bd490a3653224f7fbdf8ed2d8ad59f0de673e0d67`  
		Last Modified: Mon, 13 Mar 2023 17:17:05 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f559d903a28746e7b2cf18297c1dbd3ed8df78227b31a55764027bb8c88190`  
		Last Modified: Mon, 13 Mar 2023 17:17:03 GMT  
		Size: 10.6 KB (10638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f4bd0129aa84d8df20f9b5ed48a4a123ec3cc83121d834bc9e5e55e32a2373`  
		Last Modified: Mon, 13 Mar 2023 17:17:04 GMT  
		Size: 2.7 MB (2679912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca42b7876bf72171c45ac71c6d89f12218cc82ee2bea7227ea98efef4b97d22`  
		Last Modified: Mon, 13 Mar 2023 17:17:05 GMT  
		Size: 6.0 MB (6040868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e353d64f03127a8631c30ac73e868b707101a590d5b35332915ce50036835c`  
		Last Modified: Mon, 13 Mar 2023 17:17:03 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9ed6c536151b03b35d7e2c5575691fc2f72693d3d8ad65af13ab3414df0490`  
		Last Modified: Mon, 13 Mar 2023 17:17:03 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:latest` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:0abf618712457a362bea4768e49625dfbcb932423fb8ff4d3e48820c05eab23b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.7 MB (11687675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d3649ae583cdf8dd6866df445c5c9372471e97e2191dc50c7e96a97a2247094`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:14:57 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Fri, 10 Feb 2023 22:14:58 GMT
RUN adduser -S eggdrop
# Fri, 10 Feb 2023 22:14:59 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Fri, 10 Feb 2023 22:15:00 GMT
RUN apk add --no-cache tcl bash openssl
# Mon, 13 Mar 2023 19:46:33 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.5.tar.gz.asc eggdrop-1.9.5.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.5.tar.gz.asc   && tar -zxvf eggdrop-1.9.5.tar.gz   && rm eggdrop-1.9.5.tar.gz   && ( cd eggdrop-1.9.5     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.5   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 13 Mar 2023 19:46:33 GMT
ENV NICK=
# Mon, 13 Mar 2023 19:46:33 GMT
ENV SERVER=
# Mon, 13 Mar 2023 19:46:33 GMT
ENV LISTEN=3333
# Mon, 13 Mar 2023 19:46:33 GMT
ENV OWNER=
# Mon, 13 Mar 2023 19:46:33 GMT
ENV USERFILE=eggdrop.user
# Mon, 13 Mar 2023 19:46:33 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 13 Mar 2023 19:46:33 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 13 Mar 2023 19:46:34 GMT
EXPOSE 3333
# Mon, 13 Mar 2023 19:46:34 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Mon, 13 Mar 2023 19:46:34 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 13 Mar 2023 19:46:34 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 13 Mar 2023 19:46:34 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddb182a5cc1394eccbeeef59c5ad5d259ed5ddd4cdd2a1d4c5ad107256b7a2ee`  
		Last Modified: Fri, 10 Feb 2023 22:19:08 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59923206b30ea4054c1bb753aa8a5404a199d12f865dc365b1f8eb66fdb817b`  
		Last Modified: Fri, 10 Feb 2023 22:19:06 GMT  
		Size: 10.7 KB (10747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78dd68e4187ad121351dbe2536603e4802110332e9e21ecccff44b92d2ea68b5`  
		Last Modified: Fri, 10 Feb 2023 22:19:07 GMT  
		Size: 2.8 MB (2776467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0ddce20c0ea549cec6107f845beb13933ad23e830831793e93aa9608201939`  
		Last Modified: Mon, 13 Mar 2023 19:47:02 GMT  
		Size: 6.2 MB (6187136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93516d805e7d87b11e0b6272b3ad0d97e326a54cfc193b65a1f78193a2b105f`  
		Last Modified: Mon, 13 Mar 2023 19:47:01 GMT  
		Size: 1.8 KB (1844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00748ce261013a78b5d9d65606290d1ad4820d004dde3489c9e960d0a62846b2`  
		Last Modified: Mon, 13 Mar 2023 19:47:01 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:stable`

```console
$ docker pull eggdrop@sha256:ec2179041ce79ebd4fab44616ade6ef5eacbcc1ab3e4348990aa48b0257d7bf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:stable` - linux; amd64

```console
$ docker pull eggdrop@sha256:7d503e0bbbcf926621597e8442d5b75273ed5f51cbaebf5ca4c32e1cbca62d6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.7 MB (11707730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94885e42bceb6f392a87abdba804b2649c33d961d93aaa1cfd4ae23b75cdacdf`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:51:45 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 11 Feb 2023 07:51:46 GMT
RUN adduser -S eggdrop
# Sat, 11 Feb 2023 07:51:46 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 11 Feb 2023 07:51:48 GMT
RUN apk add --no-cache tcl bash openssl
# Sat, 11 Feb 2023 07:55:46 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.4.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.4.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.4.tar.gz.asc eggdrop-1.9.4.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.4.tar.gz.asc   && tar -zxvf eggdrop-1.9.4.tar.gz   && rm eggdrop-1.9.4.tar.gz   && ( cd eggdrop-1.9.4     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.4   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 11 Feb 2023 07:55:46 GMT
ENV NICK=
# Sat, 11 Feb 2023 07:55:46 GMT
ENV SERVER=
# Sat, 11 Feb 2023 07:55:47 GMT
ENV LISTEN=3333
# Sat, 11 Feb 2023 07:55:47 GMT
ENV OWNER=
# Sat, 11 Feb 2023 07:55:47 GMT
ENV USERFILE=eggdrop.user
# Sat, 11 Feb 2023 07:55:47 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 11 Feb 2023 07:55:47 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 11 Feb 2023 07:55:47 GMT
EXPOSE 3333
# Sat, 11 Feb 2023 07:55:47 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Sat, 11 Feb 2023 07:55:47 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 11 Feb 2023 07:55:47 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 11 Feb 2023 07:55:48 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5929d6c17ae9e3c1785e747f2e1c9a4043d1271b0b4fa46fd3b5d69e688807c3`  
		Last Modified: Sat, 11 Feb 2023 07:56:10 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45534f8d250972e326ebb489c727bd241fe3ff4b1127eb39d1d672b0168cca9e`  
		Last Modified: Sat, 11 Feb 2023 07:56:08 GMT  
		Size: 10.9 KB (10932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c10f44dd07312e4c61cf11012690bfbb08c68a17c2cbd5e4c5bec99e2dcecf`  
		Last Modified: Sat, 11 Feb 2023 07:56:09 GMT  
		Size: 2.8 MB (2757983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da126ee1240a822d73b85fe7646d08199ddab22146b346b6082d64822089bbfa`  
		Last Modified: Sat, 11 Feb 2023 07:56:09 GMT  
		Size: 6.1 MB (6127248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d97460e3eba8e8c667065808ae8282c0b7ddf147ddae13b3a5553a431bcccdd0`  
		Last Modified: Sat, 11 Feb 2023 07:56:08 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f385e4dbc86989aa993e14712f5523b1dd3458d9c4b311d202765f34873e60`  
		Last Modified: Sat, 11 Feb 2023 07:56:08 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:stable` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:add1154fcd484e80e959a680b538c3bfd2a25aedc5e2db342f32572170880ef0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.4 MB (11352013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4da83a66d4ecc8fc4b5598adbac4cd7c21311a640733c0db906a4b0b9a6a8dba`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:48 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Mon, 13 Mar 2023 16:12:48 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 17:12:15 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Mon, 13 Mar 2023 17:12:16 GMT
RUN adduser -S eggdrop
# Mon, 13 Mar 2023 17:12:17 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 13 Mar 2023 17:12:19 GMT
RUN apk add --no-cache tcl bash openssl
# Mon, 13 Mar 2023 17:16:35 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.4.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.4.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.4.tar.gz.asc eggdrop-1.9.4.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.4.tar.gz.asc   && tar -zxvf eggdrop-1.9.4.tar.gz   && rm eggdrop-1.9.4.tar.gz   && ( cd eggdrop-1.9.4     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.4   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 13 Mar 2023 17:16:35 GMT
ENV NICK=
# Mon, 13 Mar 2023 17:16:35 GMT
ENV SERVER=
# Mon, 13 Mar 2023 17:16:35 GMT
ENV LISTEN=3333
# Mon, 13 Mar 2023 17:16:36 GMT
ENV OWNER=
# Mon, 13 Mar 2023 17:16:36 GMT
ENV USERFILE=eggdrop.user
# Mon, 13 Mar 2023 17:16:36 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 13 Mar 2023 17:16:36 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 13 Mar 2023 17:16:36 GMT
EXPOSE 3333
# Mon, 13 Mar 2023 17:16:36 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Mon, 13 Mar 2023 17:16:36 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 13 Mar 2023 17:16:36 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 13 Mar 2023 17:16:36 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ec2417a5f95cb8476bdb0bd490a3653224f7fbdf8ed2d8ad59f0de673e0d67`  
		Last Modified: Mon, 13 Mar 2023 17:17:05 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f559d903a28746e7b2cf18297c1dbd3ed8df78227b31a55764027bb8c88190`  
		Last Modified: Mon, 13 Mar 2023 17:17:03 GMT  
		Size: 10.6 KB (10638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f4bd0129aa84d8df20f9b5ed48a4a123ec3cc83121d834bc9e5e55e32a2373`  
		Last Modified: Mon, 13 Mar 2023 17:17:04 GMT  
		Size: 2.7 MB (2679912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca42b7876bf72171c45ac71c6d89f12218cc82ee2bea7227ea98efef4b97d22`  
		Last Modified: Mon, 13 Mar 2023 17:17:05 GMT  
		Size: 6.0 MB (6040868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e353d64f03127a8631c30ac73e868b707101a590d5b35332915ce50036835c`  
		Last Modified: Mon, 13 Mar 2023 17:17:03 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9ed6c536151b03b35d7e2c5575691fc2f72693d3d8ad65af13ab3414df0490`  
		Last Modified: Mon, 13 Mar 2023 17:17:03 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:stable` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:0abf618712457a362bea4768e49625dfbcb932423fb8ff4d3e48820c05eab23b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.7 MB (11687675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d3649ae583cdf8dd6866df445c5c9372471e97e2191dc50c7e96a97a2247094`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:14:57 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Fri, 10 Feb 2023 22:14:58 GMT
RUN adduser -S eggdrop
# Fri, 10 Feb 2023 22:14:59 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Fri, 10 Feb 2023 22:15:00 GMT
RUN apk add --no-cache tcl bash openssl
# Mon, 13 Mar 2023 19:46:33 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.5.tar.gz.asc eggdrop-1.9.5.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.5.tar.gz.asc   && tar -zxvf eggdrop-1.9.5.tar.gz   && rm eggdrop-1.9.5.tar.gz   && ( cd eggdrop-1.9.5     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.5   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 13 Mar 2023 19:46:33 GMT
ENV NICK=
# Mon, 13 Mar 2023 19:46:33 GMT
ENV SERVER=
# Mon, 13 Mar 2023 19:46:33 GMT
ENV LISTEN=3333
# Mon, 13 Mar 2023 19:46:33 GMT
ENV OWNER=
# Mon, 13 Mar 2023 19:46:33 GMT
ENV USERFILE=eggdrop.user
# Mon, 13 Mar 2023 19:46:33 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 13 Mar 2023 19:46:33 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 13 Mar 2023 19:46:34 GMT
EXPOSE 3333
# Mon, 13 Mar 2023 19:46:34 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Mon, 13 Mar 2023 19:46:34 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 13 Mar 2023 19:46:34 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 13 Mar 2023 19:46:34 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddb182a5cc1394eccbeeef59c5ad5d259ed5ddd4cdd2a1d4c5ad107256b7a2ee`  
		Last Modified: Fri, 10 Feb 2023 22:19:08 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59923206b30ea4054c1bb753aa8a5404a199d12f865dc365b1f8eb66fdb817b`  
		Last Modified: Fri, 10 Feb 2023 22:19:06 GMT  
		Size: 10.7 KB (10747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78dd68e4187ad121351dbe2536603e4802110332e9e21ecccff44b92d2ea68b5`  
		Last Modified: Fri, 10 Feb 2023 22:19:07 GMT  
		Size: 2.8 MB (2776467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0ddce20c0ea549cec6107f845beb13933ad23e830831793e93aa9608201939`  
		Last Modified: Mon, 13 Mar 2023 19:47:02 GMT  
		Size: 6.2 MB (6187136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93516d805e7d87b11e0b6272b3ad0d97e326a54cfc193b65a1f78193a2b105f`  
		Last Modified: Mon, 13 Mar 2023 19:47:01 GMT  
		Size: 1.8 KB (1844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00748ce261013a78b5d9d65606290d1ad4820d004dde3489c9e960d0a62846b2`  
		Last Modified: Mon, 13 Mar 2023 19:47:01 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
