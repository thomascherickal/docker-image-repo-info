## `eggdrop:latest`

```console
$ docker pull eggdrop@sha256:c4f138a4862967e6f82967115f0e109bcfa5ac5bd85472fe2662db76aed7926c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:latest` - linux; amd64

```console
$ docker pull eggdrop@sha256:02687476be54e5db7a2f1d0148f0709a993091b7cb1db8df30f42309392a819a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.7 MB (11727526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8327b8ae1aa1dfccb1cd2d8163783cf913b444a2743d98c2a8777c98b775ab2`
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
# Mon, 13 Mar 2023 20:32:44 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.5.tar.gz.asc eggdrop-1.9.5.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.5.tar.gz.asc   && tar -zxvf eggdrop-1.9.5.tar.gz   && rm eggdrop-1.9.5.tar.gz   && ( cd eggdrop-1.9.5     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.5   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 13 Mar 2023 20:32:44 GMT
ENV NICK=
# Mon, 13 Mar 2023 20:32:44 GMT
ENV SERVER=
# Mon, 13 Mar 2023 20:32:44 GMT
ENV LISTEN=3333
# Mon, 13 Mar 2023 20:32:44 GMT
ENV OWNER=
# Mon, 13 Mar 2023 20:32:44 GMT
ENV USERFILE=eggdrop.user
# Mon, 13 Mar 2023 20:32:44 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 13 Mar 2023 20:32:45 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 13 Mar 2023 20:32:45 GMT
EXPOSE 3333
# Mon, 13 Mar 2023 20:32:45 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Mon, 13 Mar 2023 20:32:45 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 13 Mar 2023 20:32:45 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 13 Mar 2023 20:32:45 GMT
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
	-	`sha256:f478db3e06ff2527da0c7d1abf834862607b2528acff445545f398d76b951c71`  
		Last Modified: Mon, 13 Mar 2023 20:33:13 GMT  
		Size: 6.1 MB (6147024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd801b0966b76d02345a09662ca6be954735c46303d03234760fefbb1c23e0fa`  
		Last Modified: Mon, 13 Mar 2023 20:33:12 GMT  
		Size: 1.8 KB (1845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939b3f6e17c0e95865c3b20e9936556f6a8155b49736657cbbfe7b15fc9061ca`  
		Last Modified: Mon, 13 Mar 2023 20:33:12 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:latest` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:358c13a6e1142600283df9eb51ee33ec581e92b98c2c80a4b92098927c7e7caf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.4 MB (11365023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e1fe90a25f15ecdf5381e1a21bbaa1b6c43b49e940664bb53db4ff0853ceb38`
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
# Tue, 14 Mar 2023 04:00:01 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.5.tar.gz.asc eggdrop-1.9.5.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.5.tar.gz.asc   && tar -zxvf eggdrop-1.9.5.tar.gz   && rm eggdrop-1.9.5.tar.gz   && ( cd eggdrop-1.9.5     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.5   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Tue, 14 Mar 2023 04:00:01 GMT
ENV NICK=
# Tue, 14 Mar 2023 04:00:02 GMT
ENV SERVER=
# Tue, 14 Mar 2023 04:00:02 GMT
ENV LISTEN=3333
# Tue, 14 Mar 2023 04:00:02 GMT
ENV OWNER=
# Tue, 14 Mar 2023 04:00:02 GMT
ENV USERFILE=eggdrop.user
# Tue, 14 Mar 2023 04:00:02 GMT
ENV CHANFILE=eggdrop.chan
# Tue, 14 Mar 2023 04:00:02 GMT
WORKDIR /home/eggdrop/eggdrop
# Tue, 14 Mar 2023 04:00:02 GMT
EXPOSE 3333
# Tue, 14 Mar 2023 04:00:02 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Tue, 14 Mar 2023 04:00:02 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Tue, 14 Mar 2023 04:00:02 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Tue, 14 Mar 2023 04:00:02 GMT
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
	-	`sha256:733c834ca571f7fe000b0f4a2dce67430986c6063c3af251c6a6edc5d65ba8d4`  
		Last Modified: Tue, 14 Mar 2023 04:00:37 GMT  
		Size: 6.1 MB (6053878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf68aab61fdffc81f110cdab388b7423d44714873d5ab9fb6d444c125a49f8a7`  
		Last Modified: Tue, 14 Mar 2023 04:00:35 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc0fb5a4f6f5e599c6f2cd3abc62d77a33fe4824430aa4d14145710c06a2a8d`  
		Last Modified: Tue, 14 Mar 2023 04:00:35 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:latest` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:087798748e578aa2f07a9c8c0b984eaf308e03d9974d9ecefdf02c1ad4359344
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.7 MB (11687192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:331e0178aa41967ad6c64d6eea6323083ac3c88c4fe617fd54851779ac8095f2`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:02:16 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 29 Mar 2023 18:02:16 GMT
RUN adduser -S eggdrop
# Wed, 29 Mar 2023 18:02:17 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 29 Mar 2023 18:02:18 GMT
RUN apk add --no-cache tcl bash openssl
# Wed, 29 Mar 2023 18:06:03 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm tcl8.6.12-src.tar.gz   && rm -rf tcl8.6.12   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.5.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.5.tar.gz.asc eggdrop-1.9.5.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.5.tar.gz.asc   && tar -zxvf eggdrop-1.9.5.tar.gz   && rm eggdrop-1.9.5.tar.gz   && ( cd eggdrop-1.9.5     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.5   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 29 Mar 2023 18:06:03 GMT
ENV NICK=
# Wed, 29 Mar 2023 18:06:03 GMT
ENV SERVER=
# Wed, 29 Mar 2023 18:06:04 GMT
ENV LISTEN=3333
# Wed, 29 Mar 2023 18:06:04 GMT
ENV OWNER=
# Wed, 29 Mar 2023 18:06:04 GMT
ENV USERFILE=eggdrop.user
# Wed, 29 Mar 2023 18:06:04 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 29 Mar 2023 18:06:04 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 29 Mar 2023 18:06:04 GMT
EXPOSE 3333
# Wed, 29 Mar 2023 18:06:04 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Wed, 29 Mar 2023 18:06:04 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 29 Mar 2023 18:06:04 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 29 Mar 2023 18:06:04 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb69f3db113b0619a9372f4b7b70feb8f15fe4aa13ba9e5fa4a024ea95731f4c`  
		Last Modified: Wed, 29 Mar 2023 18:06:25 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e598031e523f6acd4c42bf753c34116e6204220d4a61ec11e62b13fb7f138160`  
		Last Modified: Wed, 29 Mar 2023 18:06:28 GMT  
		Size: 10.7 KB (10746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f2b000939306d443c2a1f2bffb5e73dbc192f7683d7b87fd89c2faedf32046`  
		Last Modified: Wed, 29 Mar 2023 18:06:24 GMT  
		Size: 2.8 MB (2776454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f270999340f5f5c78ba08b9cb807914c368554f21ed9bd0aba266124beb2d1`  
		Last Modified: Wed, 29 Mar 2023 18:06:24 GMT  
		Size: 6.2 MB (6186844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da1940fe90811d6ce6c64f3eef4eb3b53d915db33644179d48f1b8e71b8ebe4f`  
		Last Modified: Wed, 29 Mar 2023 18:06:23 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c313b4dd4c0ec3851eb42e4665a8400813ddd7d0073c923616846cb98ca2982`  
		Last Modified: Wed, 29 Mar 2023 18:06:23 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
