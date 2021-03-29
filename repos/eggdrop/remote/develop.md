## `eggdrop:develop`

```console
$ docker pull eggdrop@sha256:3560c6b621db21e28dcaf2c228228462647d517ae95c0baa82d47e7fc3c53a6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:develop` - linux; amd64

```console
$ docker pull eggdrop@sha256:8f95248afc41765a29beb58ccc1e0a9100d08d5ede19ef97409477791ca32612
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13902123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e552ecd7552a7847ed7b136a36966d161d21e02e5246469c1b4b890d74b82bc`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:43 GMT
ADD file:05adf37fc1a41a31d8e0e0b9371a01161abc0d348adacbc81689a1a34e8fe12d in / 
# Thu, 25 Mar 2021 22:19:43 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:56:54 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Fri, 26 Mar 2021 02:56:55 GMT
RUN adduser -S eggdrop
# Fri, 26 Mar 2021 02:56:56 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 29 Mar 2021 18:24:34 GMT
ENV EGGDROP_SHA256=ef482116819630aa65127d1c3d04e3762cbf45827bc66d7d505d481960209448
# Mon, 29 Mar 2021 18:24:34 GMT
ENV EGGDROP_COMMIT=d7729c4bbfb30e831e879da3985832e1db503dff
# Mon, 29 Mar 2021 18:24:36 GMT
RUN apk --update add --no-cache tcl bash openssl
# Mon, 29 Mar 2021 18:25:28 GMT
RUN apk --update add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256  develop.tar.gz" | sha256sum -c -   && tar -zxvf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 29 Mar 2021 18:25:28 GMT
ENV NICK=
# Mon, 29 Mar 2021 18:25:28 GMT
ENV SERVER=
# Mon, 29 Mar 2021 18:25:28 GMT
ENV LISTEN=3333
# Mon, 29 Mar 2021 18:25:29 GMT
ENV OWNER=
# Mon, 29 Mar 2021 18:25:29 GMT
ENV USERFILE=eggdrop.user
# Mon, 29 Mar 2021 18:25:29 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 29 Mar 2021 18:25:29 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 29 Mar 2021 18:25:29 GMT
EXPOSE 3333
# Mon, 29 Mar 2021 18:25:30 GMT
COPY file:4b2e5310f8e2b48c1ffa7bba797207637a35204a73634e98dc622889d320f394 in /home/eggdrop/eggdrop 
# Mon, 29 Mar 2021 18:25:30 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 29 Mar 2021 18:25:30 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 29 Mar 2021 18:25:30 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:839b45e0263abc8ab2dc0bfabc91a19947e932ffbd551a93970ea3ee971eadf6`  
		Last Modified: Thu, 25 Mar 2021 22:20:47 GMT  
		Size: 2.8 MB (2815332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142b4d4bcce7665a93979e1fe1f1091a8834f5695ba6201d0c301b29be4441e4`  
		Last Modified: Fri, 26 Mar 2021 02:59:30 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469ffc84df54c5381e18d169f6e0df862c133266f5b281787b3246642568fc70`  
		Last Modified: Fri, 26 Mar 2021 02:59:27 GMT  
		Size: 9.6 KB (9578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e57bf86a973cb83d31a427604abaccd148b7c853e5c6137ab144e3028213f9`  
		Last Modified: Mon, 29 Mar 2021 18:27:13 GMT  
		Size: 2.7 MB (2685239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be535f19a02b245ba61a262e0612ecc66548375af9b8454484537556810a03b`  
		Last Modified: Mon, 29 Mar 2021 18:27:17 GMT  
		Size: 8.4 MB (8388116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171725a54e3e8597c978a73daf2f84f2357054d3acd625b0d9d949d3ec800bbb`  
		Last Modified: Mon, 29 Mar 2021 18:27:12 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36fac86a2219703eededd0389b1d37904afb794fd8ae615606c08f5a811b7eb`  
		Last Modified: Mon, 29 Mar 2021 18:27:12 GMT  
		Size: 707.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:ce80af1cdfb584a75094f264d3d3a5f7c231308dc127c41d16733219e90f112e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13559937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d22d7040cd5b308e67200d0e50ef1ebd7050ca3b19e1daf5f0fe73e5b47da54`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 25 Mar 2021 22:51:39 GMT
ADD file:f9e7465b7bf9cb6b234d24519c80b22b9da7894ea0337e0ac44920114773c8a9 in / 
# Thu, 25 Mar 2021 22:51:48 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 00:18:05 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Fri, 26 Mar 2021 00:18:08 GMT
RUN adduser -S eggdrop
# Fri, 26 Mar 2021 00:18:11 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 29 Mar 2021 18:51:22 GMT
ENV EGGDROP_SHA256=ef482116819630aa65127d1c3d04e3762cbf45827bc66d7d505d481960209448
# Mon, 29 Mar 2021 18:51:23 GMT
ENV EGGDROP_COMMIT=d7729c4bbfb30e831e879da3985832e1db503dff
# Mon, 29 Mar 2021 18:51:27 GMT
RUN apk --update add --no-cache tcl bash openssl
# Mon, 29 Mar 2021 18:53:26 GMT
RUN apk --update add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256  develop.tar.gz" | sha256sum -c -   && tar -zxvf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 29 Mar 2021 18:53:27 GMT
ENV NICK=
# Mon, 29 Mar 2021 18:53:28 GMT
ENV SERVER=
# Mon, 29 Mar 2021 18:53:29 GMT
ENV LISTEN=3333
# Mon, 29 Mar 2021 18:53:29 GMT
ENV OWNER=
# Mon, 29 Mar 2021 18:53:31 GMT
ENV USERFILE=eggdrop.user
# Mon, 29 Mar 2021 18:53:32 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 29 Mar 2021 18:53:33 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 29 Mar 2021 18:53:34 GMT
EXPOSE 3333
# Mon, 29 Mar 2021 18:53:34 GMT
COPY file:4b2e5310f8e2b48c1ffa7bba797207637a35204a73634e98dc622889d320f394 in /home/eggdrop/eggdrop 
# Mon, 29 Mar 2021 18:53:35 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 29 Mar 2021 18:53:36 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 29 Mar 2021 18:53:37 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:275240b4b3a35cb935b35bfb1a8700e2b9ca100cd6e33ca8a6f83d056016bd61`  
		Last Modified: Thu, 25 Mar 2021 22:55:29 GMT  
		Size: 2.6 MB (2621328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34be1b52d02353764116f4b71c27c3531ae363dea14dd7f7ec291e807459551`  
		Last Modified: Fri, 26 Mar 2021 00:20:46 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df3fec63b7b30cda31cc85a0837f550ae13c58ce96c042da4c668890e54fc73`  
		Last Modified: Fri, 26 Mar 2021 00:20:44 GMT  
		Size: 9.4 KB (9396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f128b680f02dbe67ef96886c94570bfd2fc8344777a5a45bdc138316bfcabc`  
		Last Modified: Mon, 29 Mar 2021 18:56:40 GMT  
		Size: 2.6 MB (2608729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53788357bfe903c57109fb9a80851f2226f1313bd2a3e5fb39da8fbb01ddccf1`  
		Last Modified: Mon, 29 Mar 2021 18:56:42 GMT  
		Size: 8.3 MB (8316623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0fe9eb83df466d892892c8925e79f869731157cc5c8df28af4241d02120a21`  
		Last Modified: Mon, 29 Mar 2021 18:56:39 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8123a7a0447cb93522917f7fa914d8fdb6385d391ffccbb18ba3bd30260828dc`  
		Last Modified: Mon, 29 Mar 2021 18:56:39 GMT  
		Size: 709.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:ebe4c505999bac107006caab3087a19b1626660816a56fab4c779b4d75633749
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13868609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:175504aa01bd3ba6d34a5ed5002a36115f486789e6baf4ff32c6ca807ac190b4`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 25 Mar 2021 22:41:33 GMT
ADD file:6fca680ab44d711c282deb126e7ad2f7ab51d84a6364192a4913e178f7d393a0 in / 
# Thu, 25 Mar 2021 22:41:38 GMT
CMD ["/bin/sh"]
# Thu, 25 Mar 2021 23:57:18 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 25 Mar 2021 23:57:41 GMT
RUN adduser -S eggdrop
# Thu, 25 Mar 2021 23:58:24 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 29 Mar 2021 18:39:36 GMT
ENV EGGDROP_SHA256=ef482116819630aa65127d1c3d04e3762cbf45827bc66d7d505d481960209448
# Mon, 29 Mar 2021 18:39:36 GMT
ENV EGGDROP_COMMIT=d7729c4bbfb30e831e879da3985832e1db503dff
# Mon, 29 Mar 2021 18:39:41 GMT
RUN apk --update add --no-cache tcl bash openssl
# Mon, 29 Mar 2021 18:41:31 GMT
RUN apk --update add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256  develop.tar.gz" | sha256sum -c -   && tar -zxvf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 29 Mar 2021 18:41:32 GMT
ENV NICK=
# Mon, 29 Mar 2021 18:41:33 GMT
ENV SERVER=
# Mon, 29 Mar 2021 18:41:34 GMT
ENV LISTEN=3333
# Mon, 29 Mar 2021 18:41:35 GMT
ENV OWNER=
# Mon, 29 Mar 2021 18:41:36 GMT
ENV USERFILE=eggdrop.user
# Mon, 29 Mar 2021 18:41:38 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 29 Mar 2021 18:41:39 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 29 Mar 2021 18:41:40 GMT
EXPOSE 3333
# Mon, 29 Mar 2021 18:41:41 GMT
COPY file:4b2e5310f8e2b48c1ffa7bba797207637a35204a73634e98dc622889d320f394 in /home/eggdrop/eggdrop 
# Mon, 29 Mar 2021 18:41:42 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 29 Mar 2021 18:41:43 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 29 Mar 2021 18:41:44 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:47185b9379cb432a7a6711ec279fdcb33fe0426be145e1bf61879568c9b54054`  
		Last Modified: Thu, 25 Mar 2021 22:45:46 GMT  
		Size: 2.7 MB (2725878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:016b21c12c3099ed521797a14ada34ef399a4c317694fda20c5c7b800f40d8a6`  
		Last Modified: Fri, 26 Mar 2021 00:03:33 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002c4ae16ae920d6a492c4d547d7a976f7560f0b85134e15660d9260ba12bf09`  
		Last Modified: Fri, 26 Mar 2021 00:03:30 GMT  
		Size: 9.5 KB (9514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e65d34f70a023ecfd180699f8cc86239b7878512187ea08fe95b3251721bf1e`  
		Last Modified: Mon, 29 Mar 2021 18:44:34 GMT  
		Size: 2.7 MB (2722576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be134728433202b3225918a48165a44a5ef4b1a1c9da7f3d2e74fa50b01a8381`  
		Last Modified: Mon, 29 Mar 2021 18:44:35 GMT  
		Size: 8.4 MB (8406782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d060a30b23d1fc14460b63cd1901c866929eca6588f4d8b95fb29f8749d68cdb`  
		Last Modified: Mon, 29 Mar 2021 18:44:33 GMT  
		Size: 1.9 KB (1887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2371a756868028c8d516492b08889dad36efe78df674139a471d0fdb803279bb`  
		Last Modified: Mon, 29 Mar 2021 18:44:34 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
