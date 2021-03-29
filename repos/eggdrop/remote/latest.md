## `eggdrop:latest`

```console
$ docker pull eggdrop@sha256:53c8ef3c6dbb2599a854aa4836b127b492076cf8043fe563745a72dd24b579c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:latest` - linux; amd64

```console
$ docker pull eggdrop@sha256:13010b6a4f764c6e5425d27686195f872847ec5921a7db5a8bfc4b41168c852b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8223857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56e1b66b36045836215599980d50ddb3fd2bb467e8c4f7d66f0d70e4d82b2168`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Mon, 29 Mar 2021 18:25:37 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Mon, 29 Mar 2021 18:25:38 GMT
RUN adduser -S eggdrop
# Mon, 29 Mar 2021 18:25:39 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 29 Mar 2021 18:25:41 GMT
RUN apk add --no-cache tcl bash openssl
# Mon, 29 Mar 2021 18:26:46 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.0.tar.gz.asc eggdrop-1.9.0.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.0.tar.gz.asc   && tar -zxvf eggdrop-1.9.0.tar.gz   && rm eggdrop-1.9.0.tar.gz   && ( cd eggdrop-1.9.0     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.0   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 29 Mar 2021 18:26:46 GMT
ENV NICK=
# Mon, 29 Mar 2021 18:26:46 GMT
ENV SERVER=
# Mon, 29 Mar 2021 18:26:46 GMT
ENV LISTEN=3333
# Mon, 29 Mar 2021 18:26:46 GMT
ENV OWNER=
# Mon, 29 Mar 2021 18:26:47 GMT
ENV USERFILE=eggdrop.user
# Mon, 29 Mar 2021 18:26:47 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 29 Mar 2021 18:26:47 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 29 Mar 2021 18:26:47 GMT
EXPOSE 3333
# Mon, 29 Mar 2021 18:26:47 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Mon, 29 Mar 2021 18:26:48 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 29 Mar 2021 18:26:48 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 29 Mar 2021 18:26:48 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99eb87d40a5d04bb2f3cddc6c0113a1f4a738519880cff4f1e07f650afc6dbf3`  
		Last Modified: Mon, 29 Mar 2021 18:27:30 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0b1ed597373f415721344f92df02c7699e1e113ec744bacb5ddfe5bd3173d9`  
		Last Modified: Mon, 29 Mar 2021 18:27:28 GMT  
		Size: 10.1 KB (10109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e835b8b19e774c697d1793e108cd750e6c1892afb1297e469ba25dc9d2ba12`  
		Last Modified: Mon, 29 Mar 2021 18:27:29 GMT  
		Size: 2.7 MB (2724405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f89e026f3f26d697df684d26a88f117e9883d99d06ebeba67c6e6cfafa9e19`  
		Last Modified: Mon, 29 Mar 2021 18:27:28 GMT  
		Size: 2.7 MB (2673861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da9cf0048a0a220ae0bf1a6d07c39a67c3a4c8d8799d669b4388228680e393f`  
		Last Modified: Mon, 29 Mar 2021 18:27:28 GMT  
		Size: 1.8 KB (1839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024f150310092d715076476be109a494ac27069acdddd796376344da55c6d533`  
		Last Modified: Mon, 29 Mar 2021 18:27:28 GMT  
		Size: 698.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:latest` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:a903b3eb088fbab72e75fdbffc3792cd7311ac445dcd0bf3e914c5bf9c58e564
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7921335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5edd80bd286beab17a4624b8e275484d63f2c81eace241327185faf2a81b9e8c`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 25 Mar 2021 22:50:09 GMT
ADD file:ca4136238cb9a01d079efd129bccd1470945d7d4320da61373af90645a4b1146 in / 
# Thu, 25 Mar 2021 22:50:28 GMT
CMD ["/bin/sh"]
# Mon, 29 Mar 2021 18:53:54 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Mon, 29 Mar 2021 18:53:58 GMT
RUN adduser -S eggdrop
# Mon, 29 Mar 2021 18:54:02 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 29 Mar 2021 18:54:07 GMT
RUN apk add --no-cache tcl bash openssl
# Mon, 29 Mar 2021 18:56:09 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.0.tar.gz.asc eggdrop-1.9.0.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.0.tar.gz.asc   && tar -zxvf eggdrop-1.9.0.tar.gz   && rm eggdrop-1.9.0.tar.gz   && ( cd eggdrop-1.9.0     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.0   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 29 Mar 2021 18:56:10 GMT
ENV NICK=
# Mon, 29 Mar 2021 18:56:11 GMT
ENV SERVER=
# Mon, 29 Mar 2021 18:56:11 GMT
ENV LISTEN=3333
# Mon, 29 Mar 2021 18:56:12 GMT
ENV OWNER=
# Mon, 29 Mar 2021 18:56:13 GMT
ENV USERFILE=eggdrop.user
# Mon, 29 Mar 2021 18:56:14 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 29 Mar 2021 18:56:15 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 29 Mar 2021 18:56:15 GMT
EXPOSE 3333
# Mon, 29 Mar 2021 18:56:16 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Mon, 29 Mar 2021 18:56:17 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 29 Mar 2021 18:56:18 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 29 Mar 2021 18:56:18 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:bca6a70a54896d072b6919d2ae18d3ef685bc7aed783731f68a4adac0fb93d52`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 2.6 MB (2622062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d5795228fdf51c0b33e4b1030c55662bc5f4c74e902f62b13d97fd75eed011`  
		Last Modified: Mon, 29 Mar 2021 18:56:48 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7255637a93148079c117c136fbe895bd9664e14272e77150a651f0a20c1f0e46`  
		Last Modified: Mon, 29 Mar 2021 18:56:46 GMT  
		Size: 9.8 KB (9831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aaaae1f2c8d48c68fb8b68fb32deedb84bf83aa061a17bbc6743f44168ef65c`  
		Last Modified: Mon, 29 Mar 2021 18:56:48 GMT  
		Size: 2.7 MB (2652107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2016760df48209206db193fdf1b1870926d1e141260b961737e60d8887251c33`  
		Last Modified: Mon, 29 Mar 2021 18:56:47 GMT  
		Size: 2.6 MB (2633533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ecff28645f9741a60c783a5dae112e9afc007731f566e1f677355b27ef27d57`  
		Last Modified: Mon, 29 Mar 2021 18:56:46 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69aadba0251233b4de0d549ff16b315ec5303a767277f1b49f18f35eec7083ac`  
		Last Modified: Mon, 29 Mar 2021 18:56:46 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:latest` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:aa869560547dc520f7327b8123c108ec394137a93befa2ec96742f6c3f4e7cec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8146606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0d0f5e17e38fc11cecbc4aae1054fca1d1b46831a637640bced609cd9e10661`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 25 Mar 2021 22:40:10 GMT
ADD file:8d7431f7e3e42b162a1626e7abf4ef7605146671dccc753d490de6b7fe429261 in / 
# Thu, 25 Mar 2021 22:40:23 GMT
CMD ["/bin/sh"]
# Mon, 29 Mar 2021 18:41:56 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Mon, 29 Mar 2021 18:41:59 GMT
RUN adduser -S eggdrop
# Mon, 29 Mar 2021 18:42:04 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 29 Mar 2021 18:42:08 GMT
RUN apk add --no-cache tcl bash openssl
# Mon, 29 Mar 2021 18:44:06 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.0.tar.gz.asc   && gpg --keyserver ha.pool.sks-keyservers.net --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.0.tar.gz.asc eggdrop-1.9.0.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.0.tar.gz.asc   && tar -zxvf eggdrop-1.9.0.tar.gz   && rm eggdrop-1.9.0.tar.gz   && ( cd eggdrop-1.9.0     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.0   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 29 Mar 2021 18:44:07 GMT
ENV NICK=
# Mon, 29 Mar 2021 18:44:08 GMT
ENV SERVER=
# Mon, 29 Mar 2021 18:44:09 GMT
ENV LISTEN=3333
# Mon, 29 Mar 2021 18:44:10 GMT
ENV OWNER=
# Mon, 29 Mar 2021 18:44:10 GMT
ENV USERFILE=eggdrop.user
# Mon, 29 Mar 2021 18:44:11 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 29 Mar 2021 18:44:12 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 29 Mar 2021 18:44:13 GMT
EXPOSE 3333
# Mon, 29 Mar 2021 18:44:14 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Mon, 29 Mar 2021 18:44:15 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 29 Mar 2021 18:44:15 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 29 Mar 2021 18:44:16 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:5ceb5101e3b0d54efb5f18318982508a04b181b4d5ae52b096dd35dea3a006cc`  
		Last Modified: Thu, 25 Mar 2021 22:44:41 GMT  
		Size: 2.7 MB (2711898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7908687cab4e2e8036d3a15a7b35c59c0fb94a48df7adc80fecbf7f62b1e37f`  
		Last Modified: Mon, 29 Mar 2021 18:44:43 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed4b45bb3f885133e6216b64ea7b52fd184ceaff01b3f065710c2d4a5a75e6f`  
		Last Modified: Mon, 29 Mar 2021 18:44:42 GMT  
		Size: 10.0 KB (9994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac5efde971466056a68596f83fa25c975d505e70d57c8ab24c47c16808aaeed4`  
		Last Modified: Mon, 29 Mar 2021 18:44:42 GMT  
		Size: 2.8 MB (2752513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d1479a7f297db755dad66c514bc3a85053294cb58f8ae47793a7efaf496b9e`  
		Last Modified: Mon, 29 Mar 2021 18:44:42 GMT  
		Size: 2.7 MB (2668400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808a387447375f7ffae93dc4ee79e97f9fede109c952002b5b01d1b79b7abc1e`  
		Last Modified: Mon, 29 Mar 2021 18:44:41 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39eeef541bea0e9378eff40154ba040f95a9ac50d2c4b7f4e2b0ced63f3e1b1c`  
		Last Modified: Mon, 29 Mar 2021 18:44:41 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
