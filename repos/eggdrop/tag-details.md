<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `eggdrop`

-	[`eggdrop:1.9`](#eggdrop19)
-	[`eggdrop:1.9.3`](#eggdrop193)
-	[`eggdrop:develop`](#eggdropdevelop)
-	[`eggdrop:latest`](#eggdroplatest)
-	[`eggdrop:stable`](#eggdropstable)

## `eggdrop:1.9`

```console
$ docker pull eggdrop@sha256:4593cc4603ed97e3c71a594a9e884cbecdd29ae2aaaef3cfb6838d05aa95ae14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:1.9` - linux; amd64

```console
$ docker pull eggdrop@sha256:c83de28b71f5277ed8af3e63bf3acfa283d47632ac0c01ecffc890c629c6c2ce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8185632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:228fc31948b75db1da17173661825af496db45bbe3351395bfcb5d7e03938488`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:41:09 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 06 Oct 2022 20:41:10 GMT
RUN adduser -S eggdrop
# Thu, 06 Oct 2022 20:41:11 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 06 Oct 2022 20:41:12 GMT
RUN apk add --no-cache tcl bash openssl
# Thu, 06 Oct 2022 20:42:07 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gnupg build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.3.tar.gz.asc eggdrop-1.9.3.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.3.tar.gz.asc   && tar -zxvf eggdrop-1.9.3.tar.gz   && rm eggdrop-1.9.3.tar.gz   && ( cd eggdrop-1.9.3     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.3   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 06 Oct 2022 20:42:07 GMT
ENV NICK=
# Thu, 06 Oct 2022 20:42:07 GMT
ENV SERVER=
# Thu, 06 Oct 2022 20:42:07 GMT
ENV LISTEN=3333
# Thu, 06 Oct 2022 20:42:07 GMT
ENV OWNER=
# Thu, 06 Oct 2022 20:42:07 GMT
ENV USERFILE=eggdrop.user
# Thu, 06 Oct 2022 20:42:07 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 06 Oct 2022 20:42:07 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 06 Oct 2022 20:42:08 GMT
EXPOSE 3333
# Thu, 06 Oct 2022 20:42:08 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Thu, 06 Oct 2022 20:42:08 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 06 Oct 2022 20:42:08 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 06 Oct 2022 20:42:08 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d606fbc2174b7ed38731f6135f6e6513bb6aa77984e2b6c8b3a889a8e8729d`  
		Last Modified: Thu, 06 Oct 2022 20:42:41 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7942d93231baa07717b9e817843ce32d1d9a31c931ba96b0c0892b4ccd7149`  
		Last Modified: Thu, 06 Oct 2022 20:42:39 GMT  
		Size: 10.9 KB (10913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5b685d906f48a8f67998031e289b830b24c85bf510f0e53b381b19541dff4d`  
		Last Modified: Thu, 06 Oct 2022 20:42:39 GMT  
		Size: 2.8 MB (2757880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd43a2659f2aca61c4aa9cefe5d29c2752fb92f4ed3c8333be42b979d411984d`  
		Last Modified: Thu, 06 Oct 2022 20:42:39 GMT  
		Size: 2.6 MB (2606974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79ade8cbc13ea65d0e5b900d70c0ffd09f07f8e119b3e57e886054dd62874c53`  
		Last Modified: Thu, 06 Oct 2022 20:42:38 GMT  
		Size: 1.8 KB (1838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0818e370dc4429f9ce4643dbe34b509e14745e4e4ee6cf1b5b6b1a5fe8b9ca38`  
		Last Modified: Thu, 06 Oct 2022 20:42:39 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:1.9` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:0d64378421412fcaa3ac5fc344c6ae24caa96d3a68e6f15fc9aab12ea1345a45
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9559315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0cfafce3ce9d77ed9157950236d249dbe6ff04833718097578d756d57f29564`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:27 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Thu, 10 Nov 2022 20:49:27 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:40:45 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 10 Nov 2022 21:40:47 GMT
RUN adduser -S eggdrop
# Thu, 10 Nov 2022 21:40:49 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 10 Nov 2022 21:40:52 GMT
RUN apk add --no-cache tcl bash openssl
# Thu, 10 Nov 2022 21:42:28 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gnupg build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.3.tar.gz.asc eggdrop-1.9.3.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.3.tar.gz.asc   && tar -zxvf eggdrop-1.9.3.tar.gz   && rm eggdrop-1.9.3.tar.gz   && ( cd eggdrop-1.9.3     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.3   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 10 Nov 2022 21:42:28 GMT
ENV NICK=
# Thu, 10 Nov 2022 21:42:28 GMT
ENV SERVER=
# Thu, 10 Nov 2022 21:42:29 GMT
ENV LISTEN=3333
# Thu, 10 Nov 2022 21:42:29 GMT
ENV OWNER=
# Thu, 10 Nov 2022 21:42:29 GMT
ENV USERFILE=eggdrop.user
# Thu, 10 Nov 2022 21:42:30 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 10 Nov 2022 21:42:30 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 10 Nov 2022 21:42:31 GMT
EXPOSE 3333
# Thu, 10 Nov 2022 21:42:31 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Thu, 10 Nov 2022 21:42:32 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 10 Nov 2022 21:42:32 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 10 Nov 2022 21:42:32 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e80296a27fb59f866bf4278e334651c07eab4a0af469fb2925d13cac14d2e3`  
		Last Modified: Thu, 10 Nov 2022 21:43:20 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758852f434b05a4764a0742f301982f2b67ec99dde6ed6c29f0052df96aa9503`  
		Last Modified: Thu, 10 Nov 2022 21:43:18 GMT  
		Size: 10.6 KB (10603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826cfa6ecefe00af4ce46d705a91e9d0b3ccf1cebe3847609b710a9f2e353814`  
		Last Modified: Thu, 10 Nov 2022 21:43:19 GMT  
		Size: 2.7 MB (2679667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c06156ba57d23e1dc9ae62db477f8e6fded42b37946d9790b17ad9049ba6704`  
		Last Modified: Thu, 10 Nov 2022 21:43:19 GMT  
		Size: 4.3 MB (4251301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca67cc648b3ebf0bd586dca501a2ec68fb1f65e1fca0f78b3b56695d99f19f97`  
		Last Modified: Thu, 10 Nov 2022 21:43:18 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd3f6fb7c1bac5e20883a9315847fc8efe04b158d9a939e2c9f3f5ab64ad9d1`  
		Last Modified: Thu, 10 Nov 2022 21:43:18 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:1.9` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:c88ed874f77d380d4c8eed3428e081c66bf520a9ebf05b199a3add40fc11bc3d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9887842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5ee6e9d4f19227c1018b7100a511b402147cc57ca3c95e3ca8038aae59437df`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Thu, 10 Nov 2022 20:39:41 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 22:07:08 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 10 Nov 2022 22:07:09 GMT
RUN adduser -S eggdrop
# Thu, 10 Nov 2022 22:07:09 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 10 Nov 2022 22:07:10 GMT
RUN apk add --no-cache tcl bash openssl
# Thu, 10 Nov 2022 22:08:05 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gnupg build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.3.tar.gz.asc eggdrop-1.9.3.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.3.tar.gz.asc   && tar -zxvf eggdrop-1.9.3.tar.gz   && rm eggdrop-1.9.3.tar.gz   && ( cd eggdrop-1.9.3     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.3   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 10 Nov 2022 22:08:05 GMT
ENV NICK=
# Thu, 10 Nov 2022 22:08:05 GMT
ENV SERVER=
# Thu, 10 Nov 2022 22:08:05 GMT
ENV LISTEN=3333
# Thu, 10 Nov 2022 22:08:06 GMT
ENV OWNER=
# Thu, 10 Nov 2022 22:08:06 GMT
ENV USERFILE=eggdrop.user
# Thu, 10 Nov 2022 22:08:06 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 10 Nov 2022 22:08:06 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 10 Nov 2022 22:08:06 GMT
EXPOSE 3333
# Thu, 10 Nov 2022 22:08:06 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Thu, 10 Nov 2022 22:08:06 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 10 Nov 2022 22:08:06 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 10 Nov 2022 22:08:06 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae531d8ab57771397f121d555bba0e96be31d516bd04efc8825bf34807228bb`  
		Last Modified: Thu, 10 Nov 2022 22:08:40 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5c8f5f5aec5a839a6c58df3fc3e42bd2175dc2c9aa7d7c8b91ba693fd3f0b3`  
		Last Modified: Thu, 10 Nov 2022 22:08:39 GMT  
		Size: 10.7 KB (10712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54383a3907c5896a83dc603657f6d3b89e74ece7c22ab86bf872b85e90514deb`  
		Last Modified: Thu, 10 Nov 2022 22:08:39 GMT  
		Size: 2.8 MB (2776465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5206bf2a3db01c83d1f2af937d65454991e2d269b1b122de9ce96c5da60e9908`  
		Last Modified: Thu, 10 Nov 2022 22:08:39 GMT  
		Size: 4.4 MB (4389198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9591892ac43e2f59833af927855005cf8ce334f3e948987d3a23bde9bf9df7c1`  
		Last Modified: Thu, 10 Nov 2022 22:08:37 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4691b51b92a50226e26d84c3dadbb3988adba787073e368ff5f5e616b55203`  
		Last Modified: Thu, 10 Nov 2022 22:08:39 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:1.9.3`

```console
$ docker pull eggdrop@sha256:4593cc4603ed97e3c71a594a9e884cbecdd29ae2aaaef3cfb6838d05aa95ae14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:1.9.3` - linux; amd64

```console
$ docker pull eggdrop@sha256:c83de28b71f5277ed8af3e63bf3acfa283d47632ac0c01ecffc890c629c6c2ce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8185632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:228fc31948b75db1da17173661825af496db45bbe3351395bfcb5d7e03938488`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:41:09 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 06 Oct 2022 20:41:10 GMT
RUN adduser -S eggdrop
# Thu, 06 Oct 2022 20:41:11 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 06 Oct 2022 20:41:12 GMT
RUN apk add --no-cache tcl bash openssl
# Thu, 06 Oct 2022 20:42:07 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gnupg build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.3.tar.gz.asc eggdrop-1.9.3.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.3.tar.gz.asc   && tar -zxvf eggdrop-1.9.3.tar.gz   && rm eggdrop-1.9.3.tar.gz   && ( cd eggdrop-1.9.3     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.3   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 06 Oct 2022 20:42:07 GMT
ENV NICK=
# Thu, 06 Oct 2022 20:42:07 GMT
ENV SERVER=
# Thu, 06 Oct 2022 20:42:07 GMT
ENV LISTEN=3333
# Thu, 06 Oct 2022 20:42:07 GMT
ENV OWNER=
# Thu, 06 Oct 2022 20:42:07 GMT
ENV USERFILE=eggdrop.user
# Thu, 06 Oct 2022 20:42:07 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 06 Oct 2022 20:42:07 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 06 Oct 2022 20:42:08 GMT
EXPOSE 3333
# Thu, 06 Oct 2022 20:42:08 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Thu, 06 Oct 2022 20:42:08 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 06 Oct 2022 20:42:08 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 06 Oct 2022 20:42:08 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d606fbc2174b7ed38731f6135f6e6513bb6aa77984e2b6c8b3a889a8e8729d`  
		Last Modified: Thu, 06 Oct 2022 20:42:41 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7942d93231baa07717b9e817843ce32d1d9a31c931ba96b0c0892b4ccd7149`  
		Last Modified: Thu, 06 Oct 2022 20:42:39 GMT  
		Size: 10.9 KB (10913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5b685d906f48a8f67998031e289b830b24c85bf510f0e53b381b19541dff4d`  
		Last Modified: Thu, 06 Oct 2022 20:42:39 GMT  
		Size: 2.8 MB (2757880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd43a2659f2aca61c4aa9cefe5d29c2752fb92f4ed3c8333be42b979d411984d`  
		Last Modified: Thu, 06 Oct 2022 20:42:39 GMT  
		Size: 2.6 MB (2606974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79ade8cbc13ea65d0e5b900d70c0ffd09f07f8e119b3e57e886054dd62874c53`  
		Last Modified: Thu, 06 Oct 2022 20:42:38 GMT  
		Size: 1.8 KB (1838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0818e370dc4429f9ce4643dbe34b509e14745e4e4ee6cf1b5b6b1a5fe8b9ca38`  
		Last Modified: Thu, 06 Oct 2022 20:42:39 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:1.9.3` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:0d64378421412fcaa3ac5fc344c6ae24caa96d3a68e6f15fc9aab12ea1345a45
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9559315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0cfafce3ce9d77ed9157950236d249dbe6ff04833718097578d756d57f29564`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:27 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Thu, 10 Nov 2022 20:49:27 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:40:45 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 10 Nov 2022 21:40:47 GMT
RUN adduser -S eggdrop
# Thu, 10 Nov 2022 21:40:49 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 10 Nov 2022 21:40:52 GMT
RUN apk add --no-cache tcl bash openssl
# Thu, 10 Nov 2022 21:42:28 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gnupg build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.3.tar.gz.asc eggdrop-1.9.3.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.3.tar.gz.asc   && tar -zxvf eggdrop-1.9.3.tar.gz   && rm eggdrop-1.9.3.tar.gz   && ( cd eggdrop-1.9.3     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.3   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 10 Nov 2022 21:42:28 GMT
ENV NICK=
# Thu, 10 Nov 2022 21:42:28 GMT
ENV SERVER=
# Thu, 10 Nov 2022 21:42:29 GMT
ENV LISTEN=3333
# Thu, 10 Nov 2022 21:42:29 GMT
ENV OWNER=
# Thu, 10 Nov 2022 21:42:29 GMT
ENV USERFILE=eggdrop.user
# Thu, 10 Nov 2022 21:42:30 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 10 Nov 2022 21:42:30 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 10 Nov 2022 21:42:31 GMT
EXPOSE 3333
# Thu, 10 Nov 2022 21:42:31 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Thu, 10 Nov 2022 21:42:32 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 10 Nov 2022 21:42:32 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 10 Nov 2022 21:42:32 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e80296a27fb59f866bf4278e334651c07eab4a0af469fb2925d13cac14d2e3`  
		Last Modified: Thu, 10 Nov 2022 21:43:20 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758852f434b05a4764a0742f301982f2b67ec99dde6ed6c29f0052df96aa9503`  
		Last Modified: Thu, 10 Nov 2022 21:43:18 GMT  
		Size: 10.6 KB (10603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826cfa6ecefe00af4ce46d705a91e9d0b3ccf1cebe3847609b710a9f2e353814`  
		Last Modified: Thu, 10 Nov 2022 21:43:19 GMT  
		Size: 2.7 MB (2679667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c06156ba57d23e1dc9ae62db477f8e6fded42b37946d9790b17ad9049ba6704`  
		Last Modified: Thu, 10 Nov 2022 21:43:19 GMT  
		Size: 4.3 MB (4251301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca67cc648b3ebf0bd586dca501a2ec68fb1f65e1fca0f78b3b56695d99f19f97`  
		Last Modified: Thu, 10 Nov 2022 21:43:18 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd3f6fb7c1bac5e20883a9315847fc8efe04b158d9a939e2c9f3f5ab64ad9d1`  
		Last Modified: Thu, 10 Nov 2022 21:43:18 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:1.9.3` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:c88ed874f77d380d4c8eed3428e081c66bf520a9ebf05b199a3add40fc11bc3d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9887842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5ee6e9d4f19227c1018b7100a511b402147cc57ca3c95e3ca8038aae59437df`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Thu, 10 Nov 2022 20:39:41 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 22:07:08 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 10 Nov 2022 22:07:09 GMT
RUN adduser -S eggdrop
# Thu, 10 Nov 2022 22:07:09 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 10 Nov 2022 22:07:10 GMT
RUN apk add --no-cache tcl bash openssl
# Thu, 10 Nov 2022 22:08:05 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gnupg build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.3.tar.gz.asc eggdrop-1.9.3.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.3.tar.gz.asc   && tar -zxvf eggdrop-1.9.3.tar.gz   && rm eggdrop-1.9.3.tar.gz   && ( cd eggdrop-1.9.3     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.3   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 10 Nov 2022 22:08:05 GMT
ENV NICK=
# Thu, 10 Nov 2022 22:08:05 GMT
ENV SERVER=
# Thu, 10 Nov 2022 22:08:05 GMT
ENV LISTEN=3333
# Thu, 10 Nov 2022 22:08:06 GMT
ENV OWNER=
# Thu, 10 Nov 2022 22:08:06 GMT
ENV USERFILE=eggdrop.user
# Thu, 10 Nov 2022 22:08:06 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 10 Nov 2022 22:08:06 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 10 Nov 2022 22:08:06 GMT
EXPOSE 3333
# Thu, 10 Nov 2022 22:08:06 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Thu, 10 Nov 2022 22:08:06 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 10 Nov 2022 22:08:06 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 10 Nov 2022 22:08:06 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae531d8ab57771397f121d555bba0e96be31d516bd04efc8825bf34807228bb`  
		Last Modified: Thu, 10 Nov 2022 22:08:40 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5c8f5f5aec5a839a6c58df3fc3e42bd2175dc2c9aa7d7c8b91ba693fd3f0b3`  
		Last Modified: Thu, 10 Nov 2022 22:08:39 GMT  
		Size: 10.7 KB (10712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54383a3907c5896a83dc603657f6d3b89e74ece7c22ab86bf872b85e90514deb`  
		Last Modified: Thu, 10 Nov 2022 22:08:39 GMT  
		Size: 2.8 MB (2776465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5206bf2a3db01c83d1f2af937d65454991e2d269b1b122de9ce96c5da60e9908`  
		Last Modified: Thu, 10 Nov 2022 22:08:39 GMT  
		Size: 4.4 MB (4389198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9591892ac43e2f59833af927855005cf8ce334f3e948987d3a23bde9bf9df7c1`  
		Last Modified: Thu, 10 Nov 2022 22:08:37 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4691b51b92a50226e26d84c3dadbb3988adba787073e368ff5f5e616b55203`  
		Last Modified: Thu, 10 Nov 2022 22:08:39 GMT  
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
$ docker pull eggdrop@sha256:4593cc4603ed97e3c71a594a9e884cbecdd29ae2aaaef3cfb6838d05aa95ae14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:latest` - linux; amd64

```console
$ docker pull eggdrop@sha256:c83de28b71f5277ed8af3e63bf3acfa283d47632ac0c01ecffc890c629c6c2ce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8185632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:228fc31948b75db1da17173661825af496db45bbe3351395bfcb5d7e03938488`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:41:09 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 06 Oct 2022 20:41:10 GMT
RUN adduser -S eggdrop
# Thu, 06 Oct 2022 20:41:11 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 06 Oct 2022 20:41:12 GMT
RUN apk add --no-cache tcl bash openssl
# Thu, 06 Oct 2022 20:42:07 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gnupg build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.3.tar.gz.asc eggdrop-1.9.3.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.3.tar.gz.asc   && tar -zxvf eggdrop-1.9.3.tar.gz   && rm eggdrop-1.9.3.tar.gz   && ( cd eggdrop-1.9.3     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.3   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 06 Oct 2022 20:42:07 GMT
ENV NICK=
# Thu, 06 Oct 2022 20:42:07 GMT
ENV SERVER=
# Thu, 06 Oct 2022 20:42:07 GMT
ENV LISTEN=3333
# Thu, 06 Oct 2022 20:42:07 GMT
ENV OWNER=
# Thu, 06 Oct 2022 20:42:07 GMT
ENV USERFILE=eggdrop.user
# Thu, 06 Oct 2022 20:42:07 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 06 Oct 2022 20:42:07 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 06 Oct 2022 20:42:08 GMT
EXPOSE 3333
# Thu, 06 Oct 2022 20:42:08 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Thu, 06 Oct 2022 20:42:08 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 06 Oct 2022 20:42:08 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 06 Oct 2022 20:42:08 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d606fbc2174b7ed38731f6135f6e6513bb6aa77984e2b6c8b3a889a8e8729d`  
		Last Modified: Thu, 06 Oct 2022 20:42:41 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7942d93231baa07717b9e817843ce32d1d9a31c931ba96b0c0892b4ccd7149`  
		Last Modified: Thu, 06 Oct 2022 20:42:39 GMT  
		Size: 10.9 KB (10913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5b685d906f48a8f67998031e289b830b24c85bf510f0e53b381b19541dff4d`  
		Last Modified: Thu, 06 Oct 2022 20:42:39 GMT  
		Size: 2.8 MB (2757880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd43a2659f2aca61c4aa9cefe5d29c2752fb92f4ed3c8333be42b979d411984d`  
		Last Modified: Thu, 06 Oct 2022 20:42:39 GMT  
		Size: 2.6 MB (2606974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79ade8cbc13ea65d0e5b900d70c0ffd09f07f8e119b3e57e886054dd62874c53`  
		Last Modified: Thu, 06 Oct 2022 20:42:38 GMT  
		Size: 1.8 KB (1838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0818e370dc4429f9ce4643dbe34b509e14745e4e4ee6cf1b5b6b1a5fe8b9ca38`  
		Last Modified: Thu, 06 Oct 2022 20:42:39 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:latest` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:0d64378421412fcaa3ac5fc344c6ae24caa96d3a68e6f15fc9aab12ea1345a45
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9559315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0cfafce3ce9d77ed9157950236d249dbe6ff04833718097578d756d57f29564`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:27 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Thu, 10 Nov 2022 20:49:27 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:40:45 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 10 Nov 2022 21:40:47 GMT
RUN adduser -S eggdrop
# Thu, 10 Nov 2022 21:40:49 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 10 Nov 2022 21:40:52 GMT
RUN apk add --no-cache tcl bash openssl
# Thu, 10 Nov 2022 21:42:28 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gnupg build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.3.tar.gz.asc eggdrop-1.9.3.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.3.tar.gz.asc   && tar -zxvf eggdrop-1.9.3.tar.gz   && rm eggdrop-1.9.3.tar.gz   && ( cd eggdrop-1.9.3     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.3   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 10 Nov 2022 21:42:28 GMT
ENV NICK=
# Thu, 10 Nov 2022 21:42:28 GMT
ENV SERVER=
# Thu, 10 Nov 2022 21:42:29 GMT
ENV LISTEN=3333
# Thu, 10 Nov 2022 21:42:29 GMT
ENV OWNER=
# Thu, 10 Nov 2022 21:42:29 GMT
ENV USERFILE=eggdrop.user
# Thu, 10 Nov 2022 21:42:30 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 10 Nov 2022 21:42:30 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 10 Nov 2022 21:42:31 GMT
EXPOSE 3333
# Thu, 10 Nov 2022 21:42:31 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Thu, 10 Nov 2022 21:42:32 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 10 Nov 2022 21:42:32 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 10 Nov 2022 21:42:32 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e80296a27fb59f866bf4278e334651c07eab4a0af469fb2925d13cac14d2e3`  
		Last Modified: Thu, 10 Nov 2022 21:43:20 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758852f434b05a4764a0742f301982f2b67ec99dde6ed6c29f0052df96aa9503`  
		Last Modified: Thu, 10 Nov 2022 21:43:18 GMT  
		Size: 10.6 KB (10603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826cfa6ecefe00af4ce46d705a91e9d0b3ccf1cebe3847609b710a9f2e353814`  
		Last Modified: Thu, 10 Nov 2022 21:43:19 GMT  
		Size: 2.7 MB (2679667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c06156ba57d23e1dc9ae62db477f8e6fded42b37946d9790b17ad9049ba6704`  
		Last Modified: Thu, 10 Nov 2022 21:43:19 GMT  
		Size: 4.3 MB (4251301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca67cc648b3ebf0bd586dca501a2ec68fb1f65e1fca0f78b3b56695d99f19f97`  
		Last Modified: Thu, 10 Nov 2022 21:43:18 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd3f6fb7c1bac5e20883a9315847fc8efe04b158d9a939e2c9f3f5ab64ad9d1`  
		Last Modified: Thu, 10 Nov 2022 21:43:18 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:latest` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:c88ed874f77d380d4c8eed3428e081c66bf520a9ebf05b199a3add40fc11bc3d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9887842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5ee6e9d4f19227c1018b7100a511b402147cc57ca3c95e3ca8038aae59437df`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Thu, 10 Nov 2022 20:39:41 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 22:07:08 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 10 Nov 2022 22:07:09 GMT
RUN adduser -S eggdrop
# Thu, 10 Nov 2022 22:07:09 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 10 Nov 2022 22:07:10 GMT
RUN apk add --no-cache tcl bash openssl
# Thu, 10 Nov 2022 22:08:05 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gnupg build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.3.tar.gz.asc eggdrop-1.9.3.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.3.tar.gz.asc   && tar -zxvf eggdrop-1.9.3.tar.gz   && rm eggdrop-1.9.3.tar.gz   && ( cd eggdrop-1.9.3     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.3   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 10 Nov 2022 22:08:05 GMT
ENV NICK=
# Thu, 10 Nov 2022 22:08:05 GMT
ENV SERVER=
# Thu, 10 Nov 2022 22:08:05 GMT
ENV LISTEN=3333
# Thu, 10 Nov 2022 22:08:06 GMT
ENV OWNER=
# Thu, 10 Nov 2022 22:08:06 GMT
ENV USERFILE=eggdrop.user
# Thu, 10 Nov 2022 22:08:06 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 10 Nov 2022 22:08:06 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 10 Nov 2022 22:08:06 GMT
EXPOSE 3333
# Thu, 10 Nov 2022 22:08:06 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Thu, 10 Nov 2022 22:08:06 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 10 Nov 2022 22:08:06 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 10 Nov 2022 22:08:06 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae531d8ab57771397f121d555bba0e96be31d516bd04efc8825bf34807228bb`  
		Last Modified: Thu, 10 Nov 2022 22:08:40 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5c8f5f5aec5a839a6c58df3fc3e42bd2175dc2c9aa7d7c8b91ba693fd3f0b3`  
		Last Modified: Thu, 10 Nov 2022 22:08:39 GMT  
		Size: 10.7 KB (10712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54383a3907c5896a83dc603657f6d3b89e74ece7c22ab86bf872b85e90514deb`  
		Last Modified: Thu, 10 Nov 2022 22:08:39 GMT  
		Size: 2.8 MB (2776465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5206bf2a3db01c83d1f2af937d65454991e2d269b1b122de9ce96c5da60e9908`  
		Last Modified: Thu, 10 Nov 2022 22:08:39 GMT  
		Size: 4.4 MB (4389198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9591892ac43e2f59833af927855005cf8ce334f3e948987d3a23bde9bf9df7c1`  
		Last Modified: Thu, 10 Nov 2022 22:08:37 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4691b51b92a50226e26d84c3dadbb3988adba787073e368ff5f5e616b55203`  
		Last Modified: Thu, 10 Nov 2022 22:08:39 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eggdrop:stable`

```console
$ docker pull eggdrop@sha256:4593cc4603ed97e3c71a594a9e884cbecdd29ae2aaaef3cfb6838d05aa95ae14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:stable` - linux; amd64

```console
$ docker pull eggdrop@sha256:c83de28b71f5277ed8af3e63bf3acfa283d47632ac0c01ecffc890c629c6c2ce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8185632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:228fc31948b75db1da17173661825af496db45bbe3351395bfcb5d7e03938488`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:41:09 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 06 Oct 2022 20:41:10 GMT
RUN adduser -S eggdrop
# Thu, 06 Oct 2022 20:41:11 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 06 Oct 2022 20:41:12 GMT
RUN apk add --no-cache tcl bash openssl
# Thu, 06 Oct 2022 20:42:07 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gnupg build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.3.tar.gz.asc eggdrop-1.9.3.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.3.tar.gz.asc   && tar -zxvf eggdrop-1.9.3.tar.gz   && rm eggdrop-1.9.3.tar.gz   && ( cd eggdrop-1.9.3     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.3   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 06 Oct 2022 20:42:07 GMT
ENV NICK=
# Thu, 06 Oct 2022 20:42:07 GMT
ENV SERVER=
# Thu, 06 Oct 2022 20:42:07 GMT
ENV LISTEN=3333
# Thu, 06 Oct 2022 20:42:07 GMT
ENV OWNER=
# Thu, 06 Oct 2022 20:42:07 GMT
ENV USERFILE=eggdrop.user
# Thu, 06 Oct 2022 20:42:07 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 06 Oct 2022 20:42:07 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 06 Oct 2022 20:42:08 GMT
EXPOSE 3333
# Thu, 06 Oct 2022 20:42:08 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Thu, 06 Oct 2022 20:42:08 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 06 Oct 2022 20:42:08 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 06 Oct 2022 20:42:08 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d606fbc2174b7ed38731f6135f6e6513bb6aa77984e2b6c8b3a889a8e8729d`  
		Last Modified: Thu, 06 Oct 2022 20:42:41 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7942d93231baa07717b9e817843ce32d1d9a31c931ba96b0c0892b4ccd7149`  
		Last Modified: Thu, 06 Oct 2022 20:42:39 GMT  
		Size: 10.9 KB (10913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5b685d906f48a8f67998031e289b830b24c85bf510f0e53b381b19541dff4d`  
		Last Modified: Thu, 06 Oct 2022 20:42:39 GMT  
		Size: 2.8 MB (2757880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd43a2659f2aca61c4aa9cefe5d29c2752fb92f4ed3c8333be42b979d411984d`  
		Last Modified: Thu, 06 Oct 2022 20:42:39 GMT  
		Size: 2.6 MB (2606974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79ade8cbc13ea65d0e5b900d70c0ffd09f07f8e119b3e57e886054dd62874c53`  
		Last Modified: Thu, 06 Oct 2022 20:42:38 GMT  
		Size: 1.8 KB (1838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0818e370dc4429f9ce4643dbe34b509e14745e4e4ee6cf1b5b6b1a5fe8b9ca38`  
		Last Modified: Thu, 06 Oct 2022 20:42:39 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:stable` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:0d64378421412fcaa3ac5fc344c6ae24caa96d3a68e6f15fc9aab12ea1345a45
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9559315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0cfafce3ce9d77ed9157950236d249dbe6ff04833718097578d756d57f29564`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:27 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Thu, 10 Nov 2022 20:49:27 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:40:45 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 10 Nov 2022 21:40:47 GMT
RUN adduser -S eggdrop
# Thu, 10 Nov 2022 21:40:49 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 10 Nov 2022 21:40:52 GMT
RUN apk add --no-cache tcl bash openssl
# Thu, 10 Nov 2022 21:42:28 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gnupg build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.3.tar.gz.asc eggdrop-1.9.3.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.3.tar.gz.asc   && tar -zxvf eggdrop-1.9.3.tar.gz   && rm eggdrop-1.9.3.tar.gz   && ( cd eggdrop-1.9.3     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.3   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 10 Nov 2022 21:42:28 GMT
ENV NICK=
# Thu, 10 Nov 2022 21:42:28 GMT
ENV SERVER=
# Thu, 10 Nov 2022 21:42:29 GMT
ENV LISTEN=3333
# Thu, 10 Nov 2022 21:42:29 GMT
ENV OWNER=
# Thu, 10 Nov 2022 21:42:29 GMT
ENV USERFILE=eggdrop.user
# Thu, 10 Nov 2022 21:42:30 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 10 Nov 2022 21:42:30 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 10 Nov 2022 21:42:31 GMT
EXPOSE 3333
# Thu, 10 Nov 2022 21:42:31 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Thu, 10 Nov 2022 21:42:32 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 10 Nov 2022 21:42:32 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 10 Nov 2022 21:42:32 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e80296a27fb59f866bf4278e334651c07eab4a0af469fb2925d13cac14d2e3`  
		Last Modified: Thu, 10 Nov 2022 21:43:20 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758852f434b05a4764a0742f301982f2b67ec99dde6ed6c29f0052df96aa9503`  
		Last Modified: Thu, 10 Nov 2022 21:43:18 GMT  
		Size: 10.6 KB (10603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826cfa6ecefe00af4ce46d705a91e9d0b3ccf1cebe3847609b710a9f2e353814`  
		Last Modified: Thu, 10 Nov 2022 21:43:19 GMT  
		Size: 2.7 MB (2679667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c06156ba57d23e1dc9ae62db477f8e6fded42b37946d9790b17ad9049ba6704`  
		Last Modified: Thu, 10 Nov 2022 21:43:19 GMT  
		Size: 4.3 MB (4251301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca67cc648b3ebf0bd586dca501a2ec68fb1f65e1fca0f78b3b56695d99f19f97`  
		Last Modified: Thu, 10 Nov 2022 21:43:18 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd3f6fb7c1bac5e20883a9315847fc8efe04b158d9a939e2c9f3f5ab64ad9d1`  
		Last Modified: Thu, 10 Nov 2022 21:43:18 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:stable` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:c88ed874f77d380d4c8eed3428e081c66bf520a9ebf05b199a3add40fc11bc3d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9887842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5ee6e9d4f19227c1018b7100a511b402147cc57ca3c95e3ca8038aae59437df`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Thu, 10 Nov 2022 20:39:41 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 22:07:08 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 10 Nov 2022 22:07:09 GMT
RUN adduser -S eggdrop
# Thu, 10 Nov 2022 22:07:09 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 10 Nov 2022 22:07:10 GMT
RUN apk add --no-cache tcl bash openssl
# Thu, 10 Nov 2022 22:08:05 GMT
RUN apk add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gnupg build-base openssl-dev   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz   && wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.9/eggdrop-1.9.3.tar.gz.asc   && gpg --keyserver keyserver.ubuntu.com --recv-key E01C240484DE7DBE190FE141E7667DE1D1A39AFF   && gpg --batch --verify eggdrop-1.9.3.tar.gz.asc eggdrop-1.9.3.tar.gz   && command -v gpgconf > /dev/null   && gpgconf --kill all   && rm eggdrop-1.9.3.tar.gz.asc   && tar -zxvf eggdrop-1.9.3.tar.gz   && rm eggdrop-1.9.3.tar.gz   && ( cd eggdrop-1.9.3     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-1.9.3   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 10 Nov 2022 22:08:05 GMT
ENV NICK=
# Thu, 10 Nov 2022 22:08:05 GMT
ENV SERVER=
# Thu, 10 Nov 2022 22:08:05 GMT
ENV LISTEN=3333
# Thu, 10 Nov 2022 22:08:06 GMT
ENV OWNER=
# Thu, 10 Nov 2022 22:08:06 GMT
ENV USERFILE=eggdrop.user
# Thu, 10 Nov 2022 22:08:06 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 10 Nov 2022 22:08:06 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 10 Nov 2022 22:08:06 GMT
EXPOSE 3333
# Thu, 10 Nov 2022 22:08:06 GMT
COPY file:ddb4d88d0de0ae2531972fbd491e6c611f0bb89ff8457bc01e4e61ae7f66cd46 in /home/eggdrop/eggdrop 
# Thu, 10 Nov 2022 22:08:06 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 10 Nov 2022 22:08:06 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 10 Nov 2022 22:08:06 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae531d8ab57771397f121d555bba0e96be31d516bd04efc8825bf34807228bb`  
		Last Modified: Thu, 10 Nov 2022 22:08:40 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5c8f5f5aec5a839a6c58df3fc3e42bd2175dc2c9aa7d7c8b91ba693fd3f0b3`  
		Last Modified: Thu, 10 Nov 2022 22:08:39 GMT  
		Size: 10.7 KB (10712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54383a3907c5896a83dc603657f6d3b89e74ece7c22ab86bf872b85e90514deb`  
		Last Modified: Thu, 10 Nov 2022 22:08:39 GMT  
		Size: 2.8 MB (2776465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5206bf2a3db01c83d1f2af937d65454991e2d269b1b122de9ce96c5da60e9908`  
		Last Modified: Thu, 10 Nov 2022 22:08:39 GMT  
		Size: 4.4 MB (4389198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9591892ac43e2f59833af927855005cf8ce334f3e948987d3a23bde9bf9df7c1`  
		Last Modified: Thu, 10 Nov 2022 22:08:37 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4691b51b92a50226e26d84c3dadbb3988adba787073e368ff5f5e616b55203`  
		Last Modified: Thu, 10 Nov 2022 22:08:39 GMT  
		Size: 696.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
