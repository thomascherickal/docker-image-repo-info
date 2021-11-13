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
