## `eggdrop:develop`

```console
$ docker pull eggdrop@sha256:7495b409663c6888cd77a8e0d11b40a0cc94cc0f3ae51ac7906a30e82dd69fbd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:develop` - linux; amd64

```console
$ docker pull eggdrop@sha256:6dc7f987a543bd5af3b3630819b63c393f4b50718993b1e83d83cb922f07b5b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.8 MB (39769225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fca91a541c054b2e7ce3e6a9c5a8538842c22be50b07e940b6c413c00c1fad5e`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 18:00:24 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 23 Mar 2022 18:00:24 GMT
RUN adduser -S eggdrop
# Wed, 23 Mar 2022 18:00:25 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 23 Mar 2022 18:00:25 GMT
ENV EGGDROP_SHA256=85700bdd1e5e709e7ac44fc4cac3bf06ab674ead4fb1df99f1ba8cb892c27a3c
# Wed, 23 Mar 2022 18:00:25 GMT
ENV EGGDROP_COMMIT=6959f1943659db6117b93262d18b27dd98313206
# Wed, 23 Mar 2022 18:00:26 GMT
RUN apk --update add --no-cache bash openssl
# Wed, 23 Mar 2022 18:04:14 GMT
RUN apk --update add --no-cache --virtual egg-deps wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 23 Mar 2022 18:04:14 GMT
ENV NICK=
# Wed, 23 Mar 2022 18:04:14 GMT
ENV SERVER=
# Wed, 23 Mar 2022 18:04:15 GMT
ENV LISTEN=3333
# Wed, 23 Mar 2022 18:04:15 GMT
ENV OWNER=
# Wed, 23 Mar 2022 18:04:15 GMT
ENV USERFILE=eggdrop.user
# Wed, 23 Mar 2022 18:04:15 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 23 Mar 2022 18:04:15 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 23 Mar 2022 18:04:15 GMT
EXPOSE 3333
# Wed, 23 Mar 2022 18:04:15 GMT
COPY file:adf94c8c97044786e05e265ac7a3db4da2f14483f49d1d5b4e825de9c263b6f7 in /home/eggdrop/eggdrop 
# Wed, 23 Mar 2022 18:04:15 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 23 Mar 2022 18:04:15 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 23 Mar 2022 18:04:15 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:3aa4d0bbde192bfaba75f2d124d8cf2e6de452ae03e55d54105e46b06eb8127e`  
		Last Modified: Wed, 23 Mar 2022 15:21:44 GMT  
		Size: 2.8 MB (2812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:255d707abd67e2212c0fc03a42dec647e762d447679bc356b91ee54e0d6a2279`  
		Last Modified: Wed, 23 Mar 2022 18:04:46 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14c34e2c83cb8386f15d815f78551415b0902c87b29d55d6cf6d927d447e905`  
		Last Modified: Wed, 23 Mar 2022 18:04:43 GMT  
		Size: 11.0 KB (10951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5822447b6736a6926d59167c3028d4b67485d04cb49b0d51c1f9f9a56de5a2d`  
		Last Modified: Wed, 23 Mar 2022 18:04:44 GMT  
		Size: 1.1 MB (1089640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd5c879203d7fc23ea2576276c36cb94b1eb1bc2145bb9ab0604d2ce145fac6`  
		Last Modified: Wed, 23 Mar 2022 18:04:49 GMT  
		Size: 35.9 MB (35852104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5a15c9f725267f25678469c1126908993d96012c017bdc13a955eb42a79674`  
		Last Modified: Wed, 23 Mar 2022 18:04:43 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7d93b5f91d9637631b5c443044c61c7f7985d546ad0b9ed44d60dbc72c2222`  
		Last Modified: Wed, 23 Mar 2022 18:04:43 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:27f37eb9c752253ee4bde14b7a08dbdca44b665dcc201c9557263b8de458d7e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.2 MB (39168806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b56174b0f105dd4699df029abe3f520a415e7da53575c8a72475addaa613fa4`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 23 Mar 2022 15:49:35 GMT
ADD file:fd7f6da4a48df653ae6dd18e6d5959008daf5ce429845c974982dc7d213342d9 in / 
# Wed, 23 Mar 2022 15:49:35 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 19:06:53 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 23 Mar 2022 19:06:55 GMT
RUN adduser -S eggdrop
# Wed, 23 Mar 2022 19:06:57 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 23 Mar 2022 19:06:58 GMT
ENV EGGDROP_SHA256=85700bdd1e5e709e7ac44fc4cac3bf06ab674ead4fb1df99f1ba8cb892c27a3c
# Wed, 23 Mar 2022 19:06:58 GMT
ENV EGGDROP_COMMIT=6959f1943659db6117b93262d18b27dd98313206
# Wed, 23 Mar 2022 19:07:00 GMT
RUN apk --update add --no-cache bash openssl
# Wed, 23 Mar 2022 19:17:14 GMT
RUN apk --update add --no-cache --virtual egg-deps wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 23 Mar 2022 19:17:15 GMT
ENV NICK=
# Wed, 23 Mar 2022 19:17:15 GMT
ENV SERVER=
# Wed, 23 Mar 2022 19:17:16 GMT
ENV LISTEN=3333
# Wed, 23 Mar 2022 19:17:16 GMT
ENV OWNER=
# Wed, 23 Mar 2022 19:17:16 GMT
ENV USERFILE=eggdrop.user
# Wed, 23 Mar 2022 19:17:17 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 23 Mar 2022 19:17:17 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 23 Mar 2022 19:17:18 GMT
EXPOSE 3333
# Wed, 23 Mar 2022 19:17:18 GMT
COPY file:adf94c8c97044786e05e265ac7a3db4da2f14483f49d1d5b4e825de9c263b6f7 in /home/eggdrop/eggdrop 
# Wed, 23 Mar 2022 19:17:19 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 23 Mar 2022 19:17:19 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 23 Mar 2022 19:17:20 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:4e012d7cd81aa4570d9d209a75131b32f34a3533d5d449d23fd875513922588e`  
		Last Modified: Wed, 23 Mar 2022 15:51:07 GMT  
		Size: 2.6 MB (2624816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:965e56d6e8a96c88d0f2e343e906f0f47708d69c6c7ba96170539e225d9a1327`  
		Last Modified: Wed, 23 Mar 2022 19:18:11 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9e393b2f7b36b3a8f977f997113293e5cc6eb8be0bc20f33da61dedb0cb983`  
		Last Modified: Wed, 23 Mar 2022 19:18:10 GMT  
		Size: 10.7 KB (10652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13eb94631bb879fe11051546544fe4d36f813d5d6a07d14a2979b6f391888c2c`  
		Last Modified: Wed, 23 Mar 2022 19:18:11 GMT  
		Size: 1.0 MB (1032367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d923ce278658b2f5f2cb82a065495eb0dca24b60f271eb0e59e0c668ea11c311`  
		Last Modified: Wed, 23 Mar 2022 19:18:33 GMT  
		Size: 35.5 MB (35497119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8befdb0d8e2a12810a2081e45a6695415d67b868ece4ef870717113a0e265967`  
		Last Modified: Wed, 23 Mar 2022 19:18:10 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23a7e899a3c002c1efb9193807175661e713ea81fbf230c1725f3494bef21c9f`  
		Last Modified: Wed, 23 Mar 2022 19:18:10 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:d0a929ef427192b69a8d46b58c69795d66a2bb3d576fa139e5f67df6ac419cd4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.8 MB (39838531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:479af0ffbdfb008f646b611a5ca182fd0afbe940474b3034e6877bbaf64f9bcf`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 24 Mar 2022 00:36:14 GMT
ADD file:30da1868f9f0555fb3e5223cd75cbf3c31760c1b6087f42d78abb08a8c5066ff in / 
# Thu, 24 Mar 2022 00:36:14 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 05:09:45 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 24 Mar 2022 05:09:46 GMT
RUN adduser -S eggdrop
# Thu, 24 Mar 2022 05:09:47 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 24 Mar 2022 05:09:48 GMT
ENV EGGDROP_SHA256=85700bdd1e5e709e7ac44fc4cac3bf06ab674ead4fb1df99f1ba8cb892c27a3c
# Thu, 24 Mar 2022 05:09:49 GMT
ENV EGGDROP_COMMIT=6959f1943659db6117b93262d18b27dd98313206
# Thu, 24 Mar 2022 05:09:50 GMT
RUN apk --update add --no-cache bash openssl
# Thu, 24 Mar 2022 05:14:25 GMT
RUN apk --update add --no-cache --virtual egg-deps wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.12-src.tar.gz" -O tcl8.6.12-src.tar.gz   && tar -zxf tcl8.6.12-src.tar.gz   && ( cd tcl8.6.12     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 24 Mar 2022 05:14:25 GMT
ENV NICK=
# Thu, 24 Mar 2022 05:14:26 GMT
ENV SERVER=
# Thu, 24 Mar 2022 05:14:27 GMT
ENV LISTEN=3333
# Thu, 24 Mar 2022 05:14:28 GMT
ENV OWNER=
# Thu, 24 Mar 2022 05:14:29 GMT
ENV USERFILE=eggdrop.user
# Thu, 24 Mar 2022 05:14:30 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 24 Mar 2022 05:14:31 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 24 Mar 2022 05:14:32 GMT
EXPOSE 3333
# Thu, 24 Mar 2022 05:14:34 GMT
COPY file:adf94c8c97044786e05e265ac7a3db4da2f14483f49d1d5b4e825de9c263b6f7 in /home/eggdrop/eggdrop 
# Thu, 24 Mar 2022 05:14:35 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 24 Mar 2022 05:14:35 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 24 Mar 2022 05:14:36 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:a5e44472bb1f0d721d23f82fa10a4c3d25994790238a173c1de950a649eb9a90`  
		Last Modified: Wed, 23 Mar 2022 20:10:33 GMT  
		Size: 2.7 MB (2714720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b92d91ef5604aa6e111155577809aab2aced2a26845776cd2c773c5c98e79a1`  
		Last Modified: Thu, 24 Mar 2022 05:15:02 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b03347ecda5c13c2c0f9eb606388d846582e9f73524377dfac6903c60517e21`  
		Last Modified: Thu, 24 Mar 2022 05:15:00 GMT  
		Size: 10.7 KB (10671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a899e7ef52155c77836fd4652ba64c5a48bf1103cf17dd758252a9427bfd06a9`  
		Last Modified: Thu, 24 Mar 2022 05:15:00 GMT  
		Size: 1.1 MB (1087185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc2e3fd0cd7ed5aeeaf0b3e4064f5a3f9085ed3e7592185f1b506e1ed113086`  
		Last Modified: Thu, 24 Mar 2022 05:15:06 GMT  
		Size: 36.0 MB (36022125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f027493c578e97be9ca98c58e40135165aac7e7e0ce1ac9ede0702c72517253d`  
		Last Modified: Thu, 24 Mar 2022 05:15:00 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38dca678f81b40c9820012fc3f8f4454f84651583820ff9c2ca3b8816949584`  
		Last Modified: Thu, 24 Mar 2022 05:15:00 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
