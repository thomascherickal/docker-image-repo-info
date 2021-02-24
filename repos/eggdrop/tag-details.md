<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `eggdrop`

-	[`eggdrop:1.8`](#eggdrop18)
-	[`eggdrop:1.8.4`](#eggdrop184)
-	[`eggdrop:develop`](#eggdropdevelop)
-	[`eggdrop:latest`](#eggdroplatest)
-	[`eggdrop:stable`](#eggdropstable)

## `eggdrop:1.8`

```console
$ docker pull eggdrop@sha256:a6ca28c7d73fc33210551e9c65c01aa06a6402ca118fb2c531daf66043c3ec8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `eggdrop:1.8` - linux; amd64

```console
$ docker pull eggdrop@sha256:d26fd4c79ce1c4b7e82ad70fb7303cf690123d803c94f96ce43f2a84e306a12e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8799253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d74a600fb974d04a6dc9a6bdef409bb6d279f2432bdb9822b3be6739919b8550`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:23:46 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 24 Feb 2021 21:23:48 GMT
RUN adduser -S eggdrop
# Wed, 24 Feb 2021 21:23:50 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 24 Feb 2021 21:25:04 GMT
RUN apk add --no-cache tcl bash openssl
# Wed, 24 Feb 2021 21:26:01 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.4.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.4.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.8.4.tar.gz.asc eggdrop-1.8.4.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.8.4.tar.gz.asc   && tar -zxvf eggdrop-1.8.4.tar.gz   && rm eggdrop-1.8.4.tar.gz   && ( cd eggdrop-1.8.4     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.8.4   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 24 Feb 2021 21:26:01 GMT
ENV NICK=
# Wed, 24 Feb 2021 21:26:02 GMT
ENV SERVER=
# Wed, 24 Feb 2021 21:26:02 GMT
ENV LISTEN=3333
# Wed, 24 Feb 2021 21:26:02 GMT
ENV OWNER=
# Wed, 24 Feb 2021 21:26:03 GMT
ENV USERFILE=eggdrop.user
# Wed, 24 Feb 2021 21:26:03 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 24 Feb 2021 21:26:03 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 24 Feb 2021 21:26:04 GMT
EXPOSE 3333
# Wed, 24 Feb 2021 21:26:04 GMT
COPY file:f8d85155d39ecdefdd2ce710ca8c1211edaffb7c3fbbde0877da166dd3aaa579 in /home/eggdrop/eggdrop 
# Wed, 24 Feb 2021 21:26:05 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 24 Feb 2021 21:26:05 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 24 Feb 2021 21:26:05 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a622212a04444901eef71ac1a5abe89e7eb5812de71c73fa5493573bf18b52`  
		Last Modified: Wed, 24 Feb 2021 21:26:27 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a4a9cd3c9326ce9d816f5be5eb6f75f0a433941031aca2506e53c19765eee3`  
		Last Modified: Wed, 24 Feb 2021 21:26:26 GMT  
		Size: 9.6 KB (9577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ff529da82cac078f140d961a8bcba76ef48eab332341b30108623aff13272d`  
		Last Modified: Wed, 24 Feb 2021 21:26:33 GMT  
		Size: 2.7 MB (2684875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a4c42c51880f6950da3a324c26129c43980066bafef802fd4fe6a4b707a04f`  
		Last Modified: Wed, 24 Feb 2021 21:26:33 GMT  
		Size: 3.3 MB (3285680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71195ccb937cabda68c51c89f70a9efffd707cee394e285d34482bbad9e7d7a`  
		Last Modified: Wed, 24 Feb 2021 21:26:32 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bc9f93dbfcf216f50cc051daab55a06ca28e2d956a31544d3601ad449314e5`  
		Last Modified: Wed, 24 Feb 2021 21:26:33 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:1.8.4`

```console
$ docker pull eggdrop@sha256:a6ca28c7d73fc33210551e9c65c01aa06a6402ca118fb2c531daf66043c3ec8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `eggdrop:1.8.4` - linux; amd64

```console
$ docker pull eggdrop@sha256:d26fd4c79ce1c4b7e82ad70fb7303cf690123d803c94f96ce43f2a84e306a12e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8799253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d74a600fb974d04a6dc9a6bdef409bb6d279f2432bdb9822b3be6739919b8550`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:23:46 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 24 Feb 2021 21:23:48 GMT
RUN adduser -S eggdrop
# Wed, 24 Feb 2021 21:23:50 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 24 Feb 2021 21:25:04 GMT
RUN apk add --no-cache tcl bash openssl
# Wed, 24 Feb 2021 21:26:01 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.4.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.4.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.8.4.tar.gz.asc eggdrop-1.8.4.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.8.4.tar.gz.asc   && tar -zxvf eggdrop-1.8.4.tar.gz   && rm eggdrop-1.8.4.tar.gz   && ( cd eggdrop-1.8.4     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.8.4   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 24 Feb 2021 21:26:01 GMT
ENV NICK=
# Wed, 24 Feb 2021 21:26:02 GMT
ENV SERVER=
# Wed, 24 Feb 2021 21:26:02 GMT
ENV LISTEN=3333
# Wed, 24 Feb 2021 21:26:02 GMT
ENV OWNER=
# Wed, 24 Feb 2021 21:26:03 GMT
ENV USERFILE=eggdrop.user
# Wed, 24 Feb 2021 21:26:03 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 24 Feb 2021 21:26:03 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 24 Feb 2021 21:26:04 GMT
EXPOSE 3333
# Wed, 24 Feb 2021 21:26:04 GMT
COPY file:f8d85155d39ecdefdd2ce710ca8c1211edaffb7c3fbbde0877da166dd3aaa579 in /home/eggdrop/eggdrop 
# Wed, 24 Feb 2021 21:26:05 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 24 Feb 2021 21:26:05 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 24 Feb 2021 21:26:05 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a622212a04444901eef71ac1a5abe89e7eb5812de71c73fa5493573bf18b52`  
		Last Modified: Wed, 24 Feb 2021 21:26:27 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a4a9cd3c9326ce9d816f5be5eb6f75f0a433941031aca2506e53c19765eee3`  
		Last Modified: Wed, 24 Feb 2021 21:26:26 GMT  
		Size: 9.6 KB (9577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ff529da82cac078f140d961a8bcba76ef48eab332341b30108623aff13272d`  
		Last Modified: Wed, 24 Feb 2021 21:26:33 GMT  
		Size: 2.7 MB (2684875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a4c42c51880f6950da3a324c26129c43980066bafef802fd4fe6a4b707a04f`  
		Last Modified: Wed, 24 Feb 2021 21:26:33 GMT  
		Size: 3.3 MB (3285680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71195ccb937cabda68c51c89f70a9efffd707cee394e285d34482bbad9e7d7a`  
		Last Modified: Wed, 24 Feb 2021 21:26:32 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bc9f93dbfcf216f50cc051daab55a06ca28e2d956a31544d3601ad449314e5`  
		Last Modified: Wed, 24 Feb 2021 21:26:33 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:develop`

```console
$ docker pull eggdrop@sha256:b3c28e0d7980aeb781dd55053abb9e267b545cf044b006b97779c72d7072ff6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:develop` - linux; amd64

```console
$ docker pull eggdrop@sha256:f2f7522c1d553396db47974bee3f18fcd91752de34d6470b33a49bd115e03496
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.2 MB (13235144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7370cd0da7a9c5fb8e8b479c6daf2941e51fcf0895b460d266218ef8818d828`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:23:46 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 24 Feb 2021 21:23:48 GMT
RUN adduser -S eggdrop
# Wed, 24 Feb 2021 21:23:50 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 24 Feb 2021 21:23:51 GMT
ENV EGGDROP_SHA256=c03b55ff977b671d5d43bfc2956294ec31bda1936ec0520b260c7e7020c6f656
# Wed, 24 Feb 2021 21:23:51 GMT
ENV EGGDROP_COMMIT=a2bd85e40c85a6dcfaf8d0f11bb7967f82ac67a1
# Wed, 24 Feb 2021 21:23:54 GMT
RUN apk --update add --no-cache tcl bash openssl
# Wed, 24 Feb 2021 21:24:55 GMT
RUN apk --update add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256  develop.tar.gz" | sha256sum -c -   && tar -zxvf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 24 Feb 2021 21:24:55 GMT
ENV NICK=
# Wed, 24 Feb 2021 21:24:56 GMT
ENV SERVER=
# Wed, 24 Feb 2021 21:24:56 GMT
ENV LISTEN=3333
# Wed, 24 Feb 2021 21:24:56 GMT
ENV OWNER=
# Wed, 24 Feb 2021 21:24:56 GMT
ENV USERFILE=eggdrop.user
# Wed, 24 Feb 2021 21:24:56 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 24 Feb 2021 21:24:57 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 24 Feb 2021 21:24:57 GMT
EXPOSE 3333
# Wed, 24 Feb 2021 21:24:57 GMT
COPY file:4b2e5310f8e2b48c1ffa7bba797207637a35204a73634e98dc622889d320f394 in /home/eggdrop/eggdrop 
# Wed, 24 Feb 2021 21:24:57 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 24 Feb 2021 21:24:57 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 24 Feb 2021 21:24:58 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a622212a04444901eef71ac1a5abe89e7eb5812de71c73fa5493573bf18b52`  
		Last Modified: Wed, 24 Feb 2021 21:26:27 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a4a9cd3c9326ce9d816f5be5eb6f75f0a433941031aca2506e53c19765eee3`  
		Last Modified: Wed, 24 Feb 2021 21:26:26 GMT  
		Size: 9.6 KB (9577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a28507ba3b1d703893d38412247659ce1e0ca8e5f4c116ead57bcf21d164b3c`  
		Last Modified: Wed, 24 Feb 2021 21:26:27 GMT  
		Size: 2.7 MB (2684856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28de84a7fec123bb2c6268e723121b4958f04f51b3f082ac22d948ed68b0dc8e`  
		Last Modified: Wed, 24 Feb 2021 21:26:29 GMT  
		Size: 7.7 MB (7721581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b2287cc307a2059cf6bdd886bed89836406563fa30b0464ee23eacb315f058`  
		Last Modified: Wed, 24 Feb 2021 21:26:28 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa2ce0434175256b1d94a88cb0364bcbf937c783285bc88ad4a763440735201`  
		Last Modified: Wed, 24 Feb 2021 21:26:26 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:6cacb0cc8579625a00fa587793165b49dac436f015a0340dbe930c86777425e9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.9 MB (12901828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a16acecdff96c633acb143dc1768fc524e456c1824a6fc124ba575f6b753bedd`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:11:55 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 17 Dec 2020 01:11:57 GMT
RUN adduser -S eggdrop
# Thu, 17 Dec 2020 01:12:00 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 17 Dec 2020 01:12:01 GMT
ENV EGGDROP_SHA256=c03b55ff977b671d5d43bfc2956294ec31bda1936ec0520b260c7e7020c6f656
# Thu, 17 Dec 2020 01:12:01 GMT
ENV EGGDROP_COMMIT=a2bd85e40c85a6dcfaf8d0f11bb7967f82ac67a1
# Thu, 17 Dec 2020 01:12:05 GMT
RUN apk --update add --no-cache tcl bash openssl
# Thu, 17 Dec 2020 01:14:03 GMT
RUN apk --update add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256  develop.tar.gz" | sha256sum -c -   && tar -zxvf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 17 Dec 2020 01:14:04 GMT
ENV NICK=
# Thu, 17 Dec 2020 01:14:05 GMT
ENV SERVER=
# Thu, 17 Dec 2020 01:14:06 GMT
ENV LISTEN=3333
# Thu, 17 Dec 2020 01:14:07 GMT
ENV OWNER=
# Thu, 17 Dec 2020 01:14:08 GMT
ENV USERFILE=eggdrop.user
# Thu, 17 Dec 2020 01:14:08 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 17 Dec 2020 01:14:09 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 17 Dec 2020 01:14:10 GMT
EXPOSE 3333
# Thu, 17 Dec 2020 01:14:10 GMT
COPY file:4b2e5310f8e2b48c1ffa7bba797207637a35204a73634e98dc622889d320f394 in /home/eggdrop/eggdrop 
# Thu, 17 Dec 2020 01:14:11 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 17 Dec 2020 01:14:12 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 17 Dec 2020 01:14:13 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:56fec67ad66eea034cf5b7d0d0ffd355c0fe87611bad132ac5a952fcaa52138b`  
		Last Modified: Wed, 16 Dec 2020 23:50:34 GMT  
		Size: 2.6 MB (2620769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246d33d7e776a09750998663c72dbd23c110005878d82ca6abe5c6dcefc0967c`  
		Last Modified: Thu, 17 Dec 2020 01:14:39 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2db78c4c9d4fc9a1b9f1c23b518a7c867aa525407d02463fe69990aa5ecc860`  
		Last Modified: Thu, 17 Dec 2020 01:14:38 GMT  
		Size: 9.4 KB (9392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86dbd5777040de4ab2583b43f8d2949eed182a6f60cdb0740546e6df35369fb4`  
		Last Modified: Thu, 17 Dec 2020 01:14:37 GMT  
		Size: 2.6 MB (2608674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb871ccf8cdbd8a91e9cc1fd2e2b981520da51ca5564ef5fe51c3c59d7fef93`  
		Last Modified: Thu, 17 Dec 2020 01:14:40 GMT  
		Size: 7.7 MB (7659149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5b7a25c9dd1601e3cfe947ad0fea862d3141aab6f35df8afb6a93633be5d4e`  
		Last Modified: Thu, 17 Dec 2020 01:14:36 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b123264128fba40c616ddca02c7408a168925ff266201d28c2dd064b6273899c`  
		Last Modified: Thu, 17 Dec 2020 01:14:36 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:71f52c23af6f2daa089fc33af9d9536c5e59b08e52eda6e5dced04c81b492d14
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.2 MB (13196522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:092efcaec504a10ec4ddba863da45dd5e9ba858beb5b6a21e2f88319b9bab29b`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:51 GMT
ADD file:f8a47118a2fe92c166c426620bb4ea0090dbf17aed269177989f6dca70438750 in / 
# Wed, 24 Feb 2021 20:39:52 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:40:21 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 24 Feb 2021 21:40:23 GMT
RUN adduser -S eggdrop
# Wed, 24 Feb 2021 21:40:25 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 24 Feb 2021 21:40:26 GMT
ENV EGGDROP_SHA256=c03b55ff977b671d5d43bfc2956294ec31bda1936ec0520b260c7e7020c6f656
# Wed, 24 Feb 2021 21:40:27 GMT
ENV EGGDROP_COMMIT=a2bd85e40c85a6dcfaf8d0f11bb7967f82ac67a1
# Wed, 24 Feb 2021 21:40:30 GMT
RUN apk --update add --no-cache tcl bash openssl
# Wed, 24 Feb 2021 21:42:19 GMT
RUN apk --update add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256  develop.tar.gz" | sha256sum -c -   && tar -zxvf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 24 Feb 2021 21:42:20 GMT
ENV NICK=
# Wed, 24 Feb 2021 21:42:21 GMT
ENV SERVER=
# Wed, 24 Feb 2021 21:42:22 GMT
ENV LISTEN=3333
# Wed, 24 Feb 2021 21:42:23 GMT
ENV OWNER=
# Wed, 24 Feb 2021 21:42:24 GMT
ENV USERFILE=eggdrop.user
# Wed, 24 Feb 2021 21:42:24 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 24 Feb 2021 21:42:25 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 24 Feb 2021 21:42:27 GMT
EXPOSE 3333
# Wed, 24 Feb 2021 21:42:28 GMT
COPY file:4b2e5310f8e2b48c1ffa7bba797207637a35204a73634e98dc622889d320f394 in /home/eggdrop/eggdrop 
# Wed, 24 Feb 2021 21:42:28 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 24 Feb 2021 21:42:30 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 24 Feb 2021 21:42:30 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:0328c39aea610966704bee2d2a1c7108816950703f98b4585083cd18f8354380`  
		Last Modified: Wed, 24 Feb 2021 20:40:35 GMT  
		Size: 2.7 MB (2725816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d7e620a18c70da62d98fd84649c1aa6e9bace50def7eb2c177a1e5bd7a5a88`  
		Last Modified: Wed, 24 Feb 2021 21:42:46 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473de84245e87f528cf9f16d91909982599e6ba23d12d914bf8aa0770f103bb4`  
		Last Modified: Wed, 24 Feb 2021 21:42:45 GMT  
		Size: 9.5 KB (9517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1799fa8d5985e242d43d030c3e54d5b524b56936a35c3e6cb66da68717dc97ea`  
		Last Modified: Wed, 24 Feb 2021 21:42:45 GMT  
		Size: 2.7 MB (2722535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8c2f7eac06eaf8d77aaa1777f7afeac03d07528ce38738b208c3f6ac16f12c`  
		Last Modified: Wed, 24 Feb 2021 21:42:46 GMT  
		Size: 7.7 MB (7734807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf252e5213cca7ba05fd7b5c490ff151967233b84462b389d30a49c6f64fd0e`  
		Last Modified: Wed, 24 Feb 2021 21:42:44 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8014ed58e96e64c1c174936c8de6d6409e392d5fa2920561f15a7050f274127b`  
		Last Modified: Wed, 24 Feb 2021 21:42:44 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:latest`

```console
$ docker pull eggdrop@sha256:a6ca28c7d73fc33210551e9c65c01aa06a6402ca118fb2c531daf66043c3ec8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `eggdrop:latest` - linux; amd64

```console
$ docker pull eggdrop@sha256:d26fd4c79ce1c4b7e82ad70fb7303cf690123d803c94f96ce43f2a84e306a12e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8799253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d74a600fb974d04a6dc9a6bdef409bb6d279f2432bdb9822b3be6739919b8550`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:23:46 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 24 Feb 2021 21:23:48 GMT
RUN adduser -S eggdrop
# Wed, 24 Feb 2021 21:23:50 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 24 Feb 2021 21:25:04 GMT
RUN apk add --no-cache tcl bash openssl
# Wed, 24 Feb 2021 21:26:01 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.4.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.4.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.8.4.tar.gz.asc eggdrop-1.8.4.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.8.4.tar.gz.asc   && tar -zxvf eggdrop-1.8.4.tar.gz   && rm eggdrop-1.8.4.tar.gz   && ( cd eggdrop-1.8.4     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.8.4   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 24 Feb 2021 21:26:01 GMT
ENV NICK=
# Wed, 24 Feb 2021 21:26:02 GMT
ENV SERVER=
# Wed, 24 Feb 2021 21:26:02 GMT
ENV LISTEN=3333
# Wed, 24 Feb 2021 21:26:02 GMT
ENV OWNER=
# Wed, 24 Feb 2021 21:26:03 GMT
ENV USERFILE=eggdrop.user
# Wed, 24 Feb 2021 21:26:03 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 24 Feb 2021 21:26:03 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 24 Feb 2021 21:26:04 GMT
EXPOSE 3333
# Wed, 24 Feb 2021 21:26:04 GMT
COPY file:f8d85155d39ecdefdd2ce710ca8c1211edaffb7c3fbbde0877da166dd3aaa579 in /home/eggdrop/eggdrop 
# Wed, 24 Feb 2021 21:26:05 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 24 Feb 2021 21:26:05 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 24 Feb 2021 21:26:05 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a622212a04444901eef71ac1a5abe89e7eb5812de71c73fa5493573bf18b52`  
		Last Modified: Wed, 24 Feb 2021 21:26:27 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a4a9cd3c9326ce9d816f5be5eb6f75f0a433941031aca2506e53c19765eee3`  
		Last Modified: Wed, 24 Feb 2021 21:26:26 GMT  
		Size: 9.6 KB (9577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ff529da82cac078f140d961a8bcba76ef48eab332341b30108623aff13272d`  
		Last Modified: Wed, 24 Feb 2021 21:26:33 GMT  
		Size: 2.7 MB (2684875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a4c42c51880f6950da3a324c26129c43980066bafef802fd4fe6a4b707a04f`  
		Last Modified: Wed, 24 Feb 2021 21:26:33 GMT  
		Size: 3.3 MB (3285680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71195ccb937cabda68c51c89f70a9efffd707cee394e285d34482bbad9e7d7a`  
		Last Modified: Wed, 24 Feb 2021 21:26:32 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bc9f93dbfcf216f50cc051daab55a06ca28e2d956a31544d3601ad449314e5`  
		Last Modified: Wed, 24 Feb 2021 21:26:33 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:stable`

```console
$ docker pull eggdrop@sha256:a6ca28c7d73fc33210551e9c65c01aa06a6402ca118fb2c531daf66043c3ec8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `eggdrop:stable` - linux; amd64

```console
$ docker pull eggdrop@sha256:d26fd4c79ce1c4b7e82ad70fb7303cf690123d803c94f96ce43f2a84e306a12e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8799253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d74a600fb974d04a6dc9a6bdef409bb6d279f2432bdb9822b3be6739919b8550`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:23:46 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 24 Feb 2021 21:23:48 GMT
RUN adduser -S eggdrop
# Wed, 24 Feb 2021 21:23:50 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 24 Feb 2021 21:25:04 GMT
RUN apk add --no-cache tcl bash openssl
# Wed, 24 Feb 2021 21:26:01 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.4.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.4.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.8.4.tar.gz.asc eggdrop-1.8.4.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.8.4.tar.gz.asc   && tar -zxvf eggdrop-1.8.4.tar.gz   && rm eggdrop-1.8.4.tar.gz   && ( cd eggdrop-1.8.4     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.8.4   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 24 Feb 2021 21:26:01 GMT
ENV NICK=
# Wed, 24 Feb 2021 21:26:02 GMT
ENV SERVER=
# Wed, 24 Feb 2021 21:26:02 GMT
ENV LISTEN=3333
# Wed, 24 Feb 2021 21:26:02 GMT
ENV OWNER=
# Wed, 24 Feb 2021 21:26:03 GMT
ENV USERFILE=eggdrop.user
# Wed, 24 Feb 2021 21:26:03 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 24 Feb 2021 21:26:03 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 24 Feb 2021 21:26:04 GMT
EXPOSE 3333
# Wed, 24 Feb 2021 21:26:04 GMT
COPY file:f8d85155d39ecdefdd2ce710ca8c1211edaffb7c3fbbde0877da166dd3aaa579 in /home/eggdrop/eggdrop 
# Wed, 24 Feb 2021 21:26:05 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 24 Feb 2021 21:26:05 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 24 Feb 2021 21:26:05 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a622212a04444901eef71ac1a5abe89e7eb5812de71c73fa5493573bf18b52`  
		Last Modified: Wed, 24 Feb 2021 21:26:27 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a4a9cd3c9326ce9d816f5be5eb6f75f0a433941031aca2506e53c19765eee3`  
		Last Modified: Wed, 24 Feb 2021 21:26:26 GMT  
		Size: 9.6 KB (9577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ff529da82cac078f140d961a8bcba76ef48eab332341b30108623aff13272d`  
		Last Modified: Wed, 24 Feb 2021 21:26:33 GMT  
		Size: 2.7 MB (2684875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a4c42c51880f6950da3a324c26129c43980066bafef802fd4fe6a4b707a04f`  
		Last Modified: Wed, 24 Feb 2021 21:26:33 GMT  
		Size: 3.3 MB (3285680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e71195ccb937cabda68c51c89f70a9efffd707cee394e285d34482bbad9e7d7a`  
		Last Modified: Wed, 24 Feb 2021 21:26:32 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80bc9f93dbfcf216f50cc051daab55a06ca28e2d956a31544d3601ad449314e5`  
		Last Modified: Wed, 24 Feb 2021 21:26:33 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
