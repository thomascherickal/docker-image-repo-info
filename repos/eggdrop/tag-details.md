<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `eggdrop`

-	[`eggdrop:1.8`](#eggdrop18)
-	[`eggdrop:1.8.4`](#eggdrop184)
-	[`eggdrop:develop`](#eggdropdevelop)
-	[`eggdrop:latest`](#eggdroplatest)
-	[`eggdrop:stable`](#eggdropstable)

## `eggdrop:1.8`

```console
$ docker pull eggdrop@sha256:59db6d0f170c6af671689ed19b09212b86839befadf95257625d83d571878de1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `eggdrop:1.8` - linux; amd64

```console
$ docker pull eggdrop@sha256:0de05f9de162e737bc9e342d449d08b910cf5db394e94aaf03c3827ed668c525
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8799076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23fc16f9d95d271337d111d9fb9e0348f0733dd1fad3c8cbc9597d7b9ba1b93c`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 14:11:26 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 17 Dec 2020 14:11:28 GMT
RUN adduser -S eggdrop
# Thu, 17 Dec 2020 14:11:30 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 17 Dec 2020 14:12:57 GMT
RUN apk add --no-cache tcl bash openssl
# Thu, 17 Dec 2020 14:13:52 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.4.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.4.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.8.4.tar.gz.asc eggdrop-1.8.4.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.8.4.tar.gz.asc   && tar -zxvf eggdrop-1.8.4.tar.gz   && rm eggdrop-1.8.4.tar.gz   && ( cd eggdrop-1.8.4     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.8.4   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 17 Dec 2020 14:13:52 GMT
ENV NICK=
# Thu, 17 Dec 2020 14:13:53 GMT
ENV SERVER=
# Thu, 17 Dec 2020 14:13:53 GMT
ENV LISTEN=3333
# Thu, 17 Dec 2020 14:13:53 GMT
ENV OWNER=
# Thu, 17 Dec 2020 14:13:53 GMT
ENV USERFILE=eggdrop.user
# Thu, 17 Dec 2020 14:13:53 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 17 Dec 2020 14:13:54 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 17 Dec 2020 14:13:54 GMT
EXPOSE 3333
# Thu, 17 Dec 2020 14:13:54 GMT
COPY file:f8d85155d39ecdefdd2ce710ca8c1211edaffb7c3fbbde0877da166dd3aaa579 in /home/eggdrop/eggdrop 
# Thu, 17 Dec 2020 14:13:54 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 17 Dec 2020 14:13:54 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 17 Dec 2020 14:13:55 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc975e750079584f74b9cfdc3c5ae0f780fbf15fa7c0e27da50d095e565403c1`  
		Last Modified: Thu, 17 Dec 2020 14:14:11 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e380f7b979953c50f7b4fef1e0b7826e84efeb06c86b600c57da12f7e898d6`  
		Last Modified: Thu, 17 Dec 2020 14:14:10 GMT  
		Size: 9.6 KB (9578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4017e5d7a7432ffced49eca070dc7fae5e805eab6df288dedec4b65f6c9aeaa2`  
		Last Modified: Thu, 17 Dec 2020 14:14:18 GMT  
		Size: 2.7 MB (2685092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594e8e40a7f6fe8ca5e371cd3a187c0ea43e8687ed1593900de6d2570b050a5b`  
		Last Modified: Thu, 17 Dec 2020 14:14:19 GMT  
		Size: 3.3 MB (3285726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870293c10157a8f2f2f93e5a3c71633812d3c83d407b8b2fbe7a7f52d86493dd`  
		Last Modified: Thu, 17 Dec 2020 14:14:17 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4404ebd7ec8f77adc5a6d9a63a69c1bb3088e84489edd900db81353cb47a26`  
		Last Modified: Thu, 17 Dec 2020 14:14:18 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:1.8.4`

```console
$ docker pull eggdrop@sha256:59db6d0f170c6af671689ed19b09212b86839befadf95257625d83d571878de1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `eggdrop:1.8.4` - linux; amd64

```console
$ docker pull eggdrop@sha256:0de05f9de162e737bc9e342d449d08b910cf5db394e94aaf03c3827ed668c525
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8799076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23fc16f9d95d271337d111d9fb9e0348f0733dd1fad3c8cbc9597d7b9ba1b93c`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 14:11:26 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 17 Dec 2020 14:11:28 GMT
RUN adduser -S eggdrop
# Thu, 17 Dec 2020 14:11:30 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 17 Dec 2020 14:12:57 GMT
RUN apk add --no-cache tcl bash openssl
# Thu, 17 Dec 2020 14:13:52 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.4.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.4.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.8.4.tar.gz.asc eggdrop-1.8.4.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.8.4.tar.gz.asc   && tar -zxvf eggdrop-1.8.4.tar.gz   && rm eggdrop-1.8.4.tar.gz   && ( cd eggdrop-1.8.4     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.8.4   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 17 Dec 2020 14:13:52 GMT
ENV NICK=
# Thu, 17 Dec 2020 14:13:53 GMT
ENV SERVER=
# Thu, 17 Dec 2020 14:13:53 GMT
ENV LISTEN=3333
# Thu, 17 Dec 2020 14:13:53 GMT
ENV OWNER=
# Thu, 17 Dec 2020 14:13:53 GMT
ENV USERFILE=eggdrop.user
# Thu, 17 Dec 2020 14:13:53 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 17 Dec 2020 14:13:54 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 17 Dec 2020 14:13:54 GMT
EXPOSE 3333
# Thu, 17 Dec 2020 14:13:54 GMT
COPY file:f8d85155d39ecdefdd2ce710ca8c1211edaffb7c3fbbde0877da166dd3aaa579 in /home/eggdrop/eggdrop 
# Thu, 17 Dec 2020 14:13:54 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 17 Dec 2020 14:13:54 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 17 Dec 2020 14:13:55 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc975e750079584f74b9cfdc3c5ae0f780fbf15fa7c0e27da50d095e565403c1`  
		Last Modified: Thu, 17 Dec 2020 14:14:11 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e380f7b979953c50f7b4fef1e0b7826e84efeb06c86b600c57da12f7e898d6`  
		Last Modified: Thu, 17 Dec 2020 14:14:10 GMT  
		Size: 9.6 KB (9578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4017e5d7a7432ffced49eca070dc7fae5e805eab6df288dedec4b65f6c9aeaa2`  
		Last Modified: Thu, 17 Dec 2020 14:14:18 GMT  
		Size: 2.7 MB (2685092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594e8e40a7f6fe8ca5e371cd3a187c0ea43e8687ed1593900de6d2570b050a5b`  
		Last Modified: Thu, 17 Dec 2020 14:14:19 GMT  
		Size: 3.3 MB (3285726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870293c10157a8f2f2f93e5a3c71633812d3c83d407b8b2fbe7a7f52d86493dd`  
		Last Modified: Thu, 17 Dec 2020 14:14:17 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4404ebd7ec8f77adc5a6d9a63a69c1bb3088e84489edd900db81353cb47a26`  
		Last Modified: Thu, 17 Dec 2020 14:14:18 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:develop`

```console
$ docker pull eggdrop@sha256:47878c915950bfa2858695f6e162874ff1e7f7624d557e2332f976a68ece74ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:develop` - linux; amd64

```console
$ docker pull eggdrop@sha256:93709e47abb9f60d19ba0a31f6ea2a1e4f6169dfe7ebd7299c570cd11061c3a3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.2 MB (13233370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a8613822043ddb05e1b9cdac14d6bdd49d7f4c2a89ccc9fd4ad5cb44f3cf5c9`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 14:11:26 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 17 Dec 2020 14:11:28 GMT
RUN adduser -S eggdrop
# Thu, 17 Dec 2020 14:11:30 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 17 Dec 2020 14:11:31 GMT
ENV EGGDROP_SHA256=c03b55ff977b671d5d43bfc2956294ec31bda1936ec0520b260c7e7020c6f656
# Thu, 17 Dec 2020 14:11:31 GMT
ENV EGGDROP_COMMIT=a2bd85e40c85a6dcfaf8d0f11bb7967f82ac67a1
# Thu, 17 Dec 2020 14:11:34 GMT
RUN apk --update add --no-cache tcl bash openssl
# Thu, 17 Dec 2020 14:12:47 GMT
RUN apk --update add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256  develop.tar.gz" | sha256sum -c -   && tar -zxvf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 17 Dec 2020 14:12:47 GMT
ENV NICK=
# Thu, 17 Dec 2020 14:12:47 GMT
ENV SERVER=
# Thu, 17 Dec 2020 14:12:48 GMT
ENV LISTEN=3333
# Thu, 17 Dec 2020 14:12:48 GMT
ENV OWNER=
# Thu, 17 Dec 2020 14:12:48 GMT
ENV USERFILE=eggdrop.user
# Thu, 17 Dec 2020 14:12:48 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 17 Dec 2020 14:12:48 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 17 Dec 2020 14:12:49 GMT
EXPOSE 3333
# Thu, 17 Dec 2020 14:12:49 GMT
COPY file:4b2e5310f8e2b48c1ffa7bba797207637a35204a73634e98dc622889d320f394 in /home/eggdrop/eggdrop 
# Thu, 17 Dec 2020 14:12:49 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 17 Dec 2020 14:12:49 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 17 Dec 2020 14:12:49 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc975e750079584f74b9cfdc3c5ae0f780fbf15fa7c0e27da50d095e565403c1`  
		Last Modified: Thu, 17 Dec 2020 14:14:11 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e380f7b979953c50f7b4fef1e0b7826e84efeb06c86b600c57da12f7e898d6`  
		Last Modified: Thu, 17 Dec 2020 14:14:10 GMT  
		Size: 9.6 KB (9578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d2988ff4fb9014600b035e955a289eef301b9781c38a3f15dabe3110bd5e7e`  
		Last Modified: Thu, 17 Dec 2020 14:14:11 GMT  
		Size: 2.7 MB (2685079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5742e544d13c6585f7dac1be9cdae26d1b8db21f6bc60dd464f099f968712878`  
		Last Modified: Thu, 17 Dec 2020 14:14:13 GMT  
		Size: 7.7 MB (7720029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c6fe634f86aef0fb4d87ea0fff5ea0b683c531580ca4ac85781a8eea5bf8311`  
		Last Modified: Thu, 17 Dec 2020 14:14:10 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebb2357d9d52a1148c11e3888de4ac9377893e79b311ce6f3191ea3afa87408`  
		Last Modified: Thu, 17 Dec 2020 14:14:10 GMT  
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
$ docker pull eggdrop@sha256:2f20bd899cf1c0fa3ddc2bc4e11ec8da8feb86566751063e5ca1773e393d6488
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.2 MB (13196257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40eed0cf9c5db647ae8f6395b95b9e7a9a8d92d0019e6e5fad19bc43ae25e444`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:32:14 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 17 Dec 2020 01:32:17 GMT
RUN adduser -S eggdrop
# Thu, 17 Dec 2020 01:32:20 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 17 Dec 2020 01:32:20 GMT
ENV EGGDROP_SHA256=c03b55ff977b671d5d43bfc2956294ec31bda1936ec0520b260c7e7020c6f656
# Thu, 17 Dec 2020 01:32:22 GMT
ENV EGGDROP_COMMIT=a2bd85e40c85a6dcfaf8d0f11bb7967f82ac67a1
# Thu, 17 Dec 2020 01:32:27 GMT
RUN apk --update add --no-cache tcl bash openssl
# Thu, 17 Dec 2020 01:34:21 GMT
RUN apk --update add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256  develop.tar.gz" | sha256sum -c -   && tar -zxvf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 17 Dec 2020 01:34:22 GMT
ENV NICK=
# Thu, 17 Dec 2020 01:34:23 GMT
ENV SERVER=
# Thu, 17 Dec 2020 01:34:25 GMT
ENV LISTEN=3333
# Thu, 17 Dec 2020 01:34:27 GMT
ENV OWNER=
# Thu, 17 Dec 2020 01:34:27 GMT
ENV USERFILE=eggdrop.user
# Thu, 17 Dec 2020 01:34:28 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 17 Dec 2020 01:34:29 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 17 Dec 2020 01:34:30 GMT
EXPOSE 3333
# Thu, 17 Dec 2020 01:34:30 GMT
COPY file:4b2e5310f8e2b48c1ffa7bba797207637a35204a73634e98dc622889d320f394 in /home/eggdrop/eggdrop 
# Thu, 17 Dec 2020 01:34:31 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 17 Dec 2020 01:34:32 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 17 Dec 2020 01:34:33 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ed9edd80b941cb09da42270ec30fac48f2e333f20c112a31ceb4f07bbc5061`  
		Last Modified: Thu, 17 Dec 2020 01:34:58 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1b41d127cfd4f5f711232eeaaaaa19a7df724524428ce4e8bb07e85e0f4d0c`  
		Last Modified: Thu, 17 Dec 2020 01:34:54 GMT  
		Size: 9.5 KB (9514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9681cad244c6e2e165bdfb21360dc94cdef99de5ed2005f727c50413e6509c6e`  
		Last Modified: Thu, 17 Dec 2020 01:34:55 GMT  
		Size: 2.7 MB (2722540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1659aaa2f15dfbcb14f3daa30f8d04e477d66145cb127066cdc1b015059582c9`  
		Last Modified: Thu, 17 Dec 2020 01:34:57 GMT  
		Size: 7.7 MB (7735136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b21fb9dfb3f62df79797c1dbd01d48f0acd8925e1cad2f29583dc3bf5cbdf1`  
		Last Modified: Thu, 17 Dec 2020 01:34:54 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d73481b5f7d9d62f99f3a4779c2629d551023fe1ea1d23ff4379582b633a7c`  
		Last Modified: Thu, 17 Dec 2020 01:34:54 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:latest`

```console
$ docker pull eggdrop@sha256:59db6d0f170c6af671689ed19b09212b86839befadf95257625d83d571878de1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `eggdrop:latest` - linux; amd64

```console
$ docker pull eggdrop@sha256:0de05f9de162e737bc9e342d449d08b910cf5db394e94aaf03c3827ed668c525
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8799076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23fc16f9d95d271337d111d9fb9e0348f0733dd1fad3c8cbc9597d7b9ba1b93c`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 14:11:26 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 17 Dec 2020 14:11:28 GMT
RUN adduser -S eggdrop
# Thu, 17 Dec 2020 14:11:30 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 17 Dec 2020 14:12:57 GMT
RUN apk add --no-cache tcl bash openssl
# Thu, 17 Dec 2020 14:13:52 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.4.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.4.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.8.4.tar.gz.asc eggdrop-1.8.4.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.8.4.tar.gz.asc   && tar -zxvf eggdrop-1.8.4.tar.gz   && rm eggdrop-1.8.4.tar.gz   && ( cd eggdrop-1.8.4     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.8.4   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 17 Dec 2020 14:13:52 GMT
ENV NICK=
# Thu, 17 Dec 2020 14:13:53 GMT
ENV SERVER=
# Thu, 17 Dec 2020 14:13:53 GMT
ENV LISTEN=3333
# Thu, 17 Dec 2020 14:13:53 GMT
ENV OWNER=
# Thu, 17 Dec 2020 14:13:53 GMT
ENV USERFILE=eggdrop.user
# Thu, 17 Dec 2020 14:13:53 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 17 Dec 2020 14:13:54 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 17 Dec 2020 14:13:54 GMT
EXPOSE 3333
# Thu, 17 Dec 2020 14:13:54 GMT
COPY file:f8d85155d39ecdefdd2ce710ca8c1211edaffb7c3fbbde0877da166dd3aaa579 in /home/eggdrop/eggdrop 
# Thu, 17 Dec 2020 14:13:54 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 17 Dec 2020 14:13:54 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 17 Dec 2020 14:13:55 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc975e750079584f74b9cfdc3c5ae0f780fbf15fa7c0e27da50d095e565403c1`  
		Last Modified: Thu, 17 Dec 2020 14:14:11 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e380f7b979953c50f7b4fef1e0b7826e84efeb06c86b600c57da12f7e898d6`  
		Last Modified: Thu, 17 Dec 2020 14:14:10 GMT  
		Size: 9.6 KB (9578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4017e5d7a7432ffced49eca070dc7fae5e805eab6df288dedec4b65f6c9aeaa2`  
		Last Modified: Thu, 17 Dec 2020 14:14:18 GMT  
		Size: 2.7 MB (2685092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594e8e40a7f6fe8ca5e371cd3a187c0ea43e8687ed1593900de6d2570b050a5b`  
		Last Modified: Thu, 17 Dec 2020 14:14:19 GMT  
		Size: 3.3 MB (3285726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870293c10157a8f2f2f93e5a3c71633812d3c83d407b8b2fbe7a7f52d86493dd`  
		Last Modified: Thu, 17 Dec 2020 14:14:17 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4404ebd7ec8f77adc5a6d9a63a69c1bb3088e84489edd900db81353cb47a26`  
		Last Modified: Thu, 17 Dec 2020 14:14:18 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:stable`

```console
$ docker pull eggdrop@sha256:59db6d0f170c6af671689ed19b09212b86839befadf95257625d83d571878de1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `eggdrop:stable` - linux; amd64

```console
$ docker pull eggdrop@sha256:0de05f9de162e737bc9e342d449d08b910cf5db394e94aaf03c3827ed668c525
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8799076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23fc16f9d95d271337d111d9fb9e0348f0733dd1fad3c8cbc9597d7b9ba1b93c`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 14:11:26 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 17 Dec 2020 14:11:28 GMT
RUN adduser -S eggdrop
# Thu, 17 Dec 2020 14:11:30 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 17 Dec 2020 14:12:57 GMT
RUN apk add --no-cache tcl bash openssl
# Thu, 17 Dec 2020 14:13:52 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.4.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.8/eggdrop-1.8.4.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.8.4.tar.gz.asc eggdrop-1.8.4.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.8.4.tar.gz.asc   && tar -zxvf eggdrop-1.8.4.tar.gz   && rm eggdrop-1.8.4.tar.gz   && ( cd eggdrop-1.8.4     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.8.4   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 17 Dec 2020 14:13:52 GMT
ENV NICK=
# Thu, 17 Dec 2020 14:13:53 GMT
ENV SERVER=
# Thu, 17 Dec 2020 14:13:53 GMT
ENV LISTEN=3333
# Thu, 17 Dec 2020 14:13:53 GMT
ENV OWNER=
# Thu, 17 Dec 2020 14:13:53 GMT
ENV USERFILE=eggdrop.user
# Thu, 17 Dec 2020 14:13:53 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 17 Dec 2020 14:13:54 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 17 Dec 2020 14:13:54 GMT
EXPOSE 3333
# Thu, 17 Dec 2020 14:13:54 GMT
COPY file:f8d85155d39ecdefdd2ce710ca8c1211edaffb7c3fbbde0877da166dd3aaa579 in /home/eggdrop/eggdrop 
# Thu, 17 Dec 2020 14:13:54 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 17 Dec 2020 14:13:54 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 17 Dec 2020 14:13:55 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc975e750079584f74b9cfdc3c5ae0f780fbf15fa7c0e27da50d095e565403c1`  
		Last Modified: Thu, 17 Dec 2020 14:14:11 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e380f7b979953c50f7b4fef1e0b7826e84efeb06c86b600c57da12f7e898d6`  
		Last Modified: Thu, 17 Dec 2020 14:14:10 GMT  
		Size: 9.6 KB (9578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4017e5d7a7432ffced49eca070dc7fae5e805eab6df288dedec4b65f6c9aeaa2`  
		Last Modified: Thu, 17 Dec 2020 14:14:18 GMT  
		Size: 2.7 MB (2685092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594e8e40a7f6fe8ca5e371cd3a187c0ea43e8687ed1593900de6d2570b050a5b`  
		Last Modified: Thu, 17 Dec 2020 14:14:19 GMT  
		Size: 3.3 MB (3285726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870293c10157a8f2f2f93e5a3c71633812d3c83d407b8b2fbe7a7f52d86493dd`  
		Last Modified: Thu, 17 Dec 2020 14:14:17 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4404ebd7ec8f77adc5a6d9a63a69c1bb3088e84489edd900db81353cb47a26`  
		Last Modified: Thu, 17 Dec 2020 14:14:18 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
