## `eggdrop:develop`

```console
$ docker pull eggdrop@sha256:ac896e6caeaac21d165f4afc4d6046fa092fbbb89f32a9be52cc07c6cf19838d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:develop` - linux; amd64

```console
$ docker pull eggdrop@sha256:894660c3e8dedfd2392249dfbc49c1fbd62e348a99991197722d874ae7ef2e48
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.2 MB (18190549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5caa6fba2a1a8ccce0c352d1a697408f686d3db0c20ed6b36cca6502a2170610`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Fri, 17 Nov 2023 01:26:35 GMT
LABEL org.opencontainers.image.authors=Geo Van O <geo@eggheads.org> org.opencontainers.image.url=https://www.eggheads.org
# Fri, 17 Nov 2023 01:26:35 GMT
RUN addgroup -S -g 3333 eggdrop     && adduser -S -u 3333 eggdrop eggdrop
# Fri, 17 Nov 2023 01:26:37 GMT
RUN apk add --no-cache 'su-exec>=0.2' bash openssl
# Fri, 17 Nov 2023 01:26:37 GMT
ENV EGGDROP_SHA256=a155625d2ac3a0673e69c9d0149293910583c1623cd1f90f38ad2bcba7b2b766
# Fri, 17 Nov 2023 01:26:37 GMT
ENV EGGDROP_COMMIT=322bddbd102d58cdb00864a3a335b086beaf042c
# Fri, 17 Nov 2023 01:28:44 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.13-src.tar.gz" -O tcl8.6.13-src.tar.gz --progress=dot:giga   && tar -zxf tcl8.6.13-src.tar.gz   && ( cd tcl8.6.13     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && nproc="$(nproc)"     && make -j"$nproc"     && make install )   && rm -rf tcl8.6.13-src.tar.gz   && rm -rf tcl8.6.13   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && nproc="$(nproc)"     && make -j"$nproc"     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del --no-network egg-deps
# Fri, 17 Nov 2023 01:28:44 GMT
ENV NICK=
# Fri, 17 Nov 2023 01:28:45 GMT
ENV SERVER=
# Fri, 17 Nov 2023 01:28:45 GMT
ENV LISTEN=3333
# Fri, 17 Nov 2023 01:28:45 GMT
ENV USERFILE=eggdrop.user
# Fri, 17 Nov 2023 01:28:45 GMT
ENV CHANFILE=eggdrop.chan
# Fri, 17 Nov 2023 01:28:45 GMT
WORKDIR /home/eggdrop/eggdrop
# Fri, 17 Nov 2023 01:28:45 GMT
EXPOSE 3333
# Fri, 17 Nov 2023 01:28:45 GMT
COPY file:15b1df22891b2d819093301ed85a114b9e76e06ecf7eba8f403edb7908e4aebf in ./ 
# Fri, 17 Nov 2023 01:28:45 GMT
COPY file:f30bcb89ff6df7709069d6cc97353d72cdbbebc6530d8d350cbb3ae4dad79129 in ./scripts/ 
# Fri, 17 Nov 2023 01:28:45 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Fri, 17 Nov 2023 01:28:45 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732219b2a89b33346f29319018d1a434342e3e73898ae738b5f4c450d2990aa4`  
		Last Modified: Fri, 17 Nov 2023 01:29:07 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee349db92ae049ac412473eb7d05a0ec92e145bdea7db3df2a930d93a8b84c7`  
		Last Modified: Fri, 17 Nov 2023 01:29:07 GMT  
		Size: 3.3 MB (3253657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076db7989bb271698eeecad89f87da2e10bf5fa45069ed121b7ae4c505a17bd8`  
		Last Modified: Fri, 17 Nov 2023 01:29:08 GMT  
		Size: 11.6 MB (11554001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3ac5f29cc83592a32bf2b2d897f091629e0006868e96bad6004ae00b8c3d798`  
		Last Modified: Fri, 17 Nov 2023 01:29:07 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9432c626d23cfbb2bd78ec905f712211833e34d66b5033cd932d3933922d31bf`  
		Last Modified: Fri, 17 Nov 2023 01:29:07 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:efadae87c1de5e32ec5ae3feaa94ad1036efb3c68fcc7d0ebe87048259ade9c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15746145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72a40062f619d324347fe62da0cfa525c5ce5637d14878fcfe8a16530bdfcf0f`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:21 GMT
ADD file:90d3bdc6a557ead63796de0110e2fda87e65aa091070cbae612dfb2126568253 in / 
# Thu, 30 Nov 2023 22:49:21 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 00:44:28 GMT
LABEL org.opencontainers.image.authors=Geo Van O <geo@eggheads.org> org.opencontainers.image.url=https://www.eggheads.org
# Fri, 01 Dec 2023 00:44:29 GMT
RUN addgroup -S -g 3333 eggdrop     && adduser -S -u 3333 eggdrop eggdrop
# Fri, 01 Dec 2023 00:44:30 GMT
RUN apk add --no-cache 'su-exec>=0.2' bash openssl
# Fri, 01 Dec 2023 00:44:30 GMT
ENV EGGDROP_SHA256=a155625d2ac3a0673e69c9d0149293910583c1623cd1f90f38ad2bcba7b2b766
# Fri, 01 Dec 2023 00:44:30 GMT
ENV EGGDROP_COMMIT=322bddbd102d58cdb00864a3a335b086beaf042c
# Fri, 01 Dec 2023 00:46:45 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.13-src.tar.gz" -O tcl8.6.13-src.tar.gz --progress=dot:giga   && tar -zxf tcl8.6.13-src.tar.gz   && ( cd tcl8.6.13     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && nproc="$(nproc)"     && make -j"$nproc"     && make install )   && rm -rf tcl8.6.13-src.tar.gz   && rm -rf tcl8.6.13   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && nproc="$(nproc)"     && make -j"$nproc"     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del --no-network egg-deps
# Fri, 01 Dec 2023 00:46:45 GMT
ENV NICK=
# Fri, 01 Dec 2023 00:46:45 GMT
ENV SERVER=
# Fri, 01 Dec 2023 00:46:45 GMT
ENV LISTEN=3333
# Fri, 01 Dec 2023 00:46:45 GMT
ENV USERFILE=eggdrop.user
# Fri, 01 Dec 2023 00:46:46 GMT
ENV CHANFILE=eggdrop.chan
# Fri, 01 Dec 2023 00:46:46 GMT
WORKDIR /home/eggdrop/eggdrop
# Fri, 01 Dec 2023 00:46:46 GMT
EXPOSE 3333
# Fri, 01 Dec 2023 00:46:46 GMT
COPY file:15b1df22891b2d819093301ed85a114b9e76e06ecf7eba8f403edb7908e4aebf in ./ 
# Fri, 01 Dec 2023 00:46:46 GMT
COPY file:f30bcb89ff6df7709069d6cc97353d72cdbbebc6530d8d350cbb3ae4dad79129 in ./scripts/ 
# Fri, 01 Dec 2023 00:46:46 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Fri, 01 Dec 2023 00:46:46 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:f0440ff44d712e5fc701b84856116589b428157893ac461b633b1ab30b627eed`  
		Last Modified: Thu, 30 Nov 2023 22:49:52 GMT  
		Size: 3.1 MB (3113003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2007141e1acfb13278961b1dd692cc8a98a7e1b62eeaff37f1adbb12e8430e42`  
		Last Modified: Fri, 01 Dec 2023 00:51:36 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468e6c2f98a7e7b040cfec6a1355ead740cfd1a1808df7dbd49a65179c31bf27`  
		Last Modified: Fri, 01 Dec 2023 00:51:35 GMT  
		Size: 1.2 MB (1190279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c6293eb2d227b278db01528877de24f462ee047e43c001dca3e2fb96b50088`  
		Last Modified: Fri, 01 Dec 2023 00:51:37 GMT  
		Size: 11.4 MB (11438578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3cf3ee2be1b239ea78d66ba74bda662c437d4bc32f1e42dc04cc83c5076c289`  
		Last Modified: Fri, 01 Dec 2023 00:51:35 GMT  
		Size: 2.0 KB (1951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8382e1ecf17320063154e4d3958995df68ef0b8e7330a1d167d7ba6a06d44fde`  
		Last Modified: Fri, 01 Dec 2023 00:51:35 GMT  
		Size: 1.1 KB (1059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:2b51503441c8d0ad8c293063e01ee3c6f71ecf9378d9ecd196e113aecdaa7519
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.0 MB (18014357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c036cf0a7b8624cbbafb8927c59054c637141b2798495b982c2dc35e1d348eb9`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:22 GMT
ADD file:9e054a25c83111adc857a7f988336ee40eea5e1794ed30a80d465e8d472342e2 in / 
# Mon, 07 Aug 2023 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 17 Nov 2023 00:44:19 GMT
LABEL org.opencontainers.image.authors=Geo Van O <geo@eggheads.org> org.opencontainers.image.url=https://www.eggheads.org
# Fri, 17 Nov 2023 00:44:20 GMT
RUN addgroup -S -g 3333 eggdrop     && adduser -S -u 3333 eggdrop eggdrop
# Fri, 17 Nov 2023 00:44:21 GMT
RUN apk add --no-cache 'su-exec>=0.2' bash openssl
# Fri, 17 Nov 2023 00:44:21 GMT
ENV EGGDROP_SHA256=a155625d2ac3a0673e69c9d0149293910583c1623cd1f90f38ad2bcba7b2b766
# Fri, 17 Nov 2023 00:44:21 GMT
ENV EGGDROP_COMMIT=322bddbd102d58cdb00864a3a335b086beaf042c
# Fri, 17 Nov 2023 00:46:09 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.13-src.tar.gz" -O tcl8.6.13-src.tar.gz --progress=dot:giga   && tar -zxf tcl8.6.13-src.tar.gz   && ( cd tcl8.6.13     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && nproc="$(nproc)"     && make -j"$nproc"     && make install )   && rm -rf tcl8.6.13-src.tar.gz   && rm -rf tcl8.6.13   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && nproc="$(nproc)"     && make -j"$nproc"     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del --no-network egg-deps
# Fri, 17 Nov 2023 00:46:09 GMT
ENV NICK=
# Fri, 17 Nov 2023 00:46:09 GMT
ENV SERVER=
# Fri, 17 Nov 2023 00:46:09 GMT
ENV LISTEN=3333
# Fri, 17 Nov 2023 00:46:09 GMT
ENV USERFILE=eggdrop.user
# Fri, 17 Nov 2023 00:46:10 GMT
ENV CHANFILE=eggdrop.chan
# Fri, 17 Nov 2023 00:46:10 GMT
WORKDIR /home/eggdrop/eggdrop
# Fri, 17 Nov 2023 00:46:10 GMT
EXPOSE 3333
# Fri, 17 Nov 2023 00:46:10 GMT
COPY file:15b1df22891b2d819093301ed85a114b9e76e06ecf7eba8f403edb7908e4aebf in ./ 
# Fri, 17 Nov 2023 00:46:10 GMT
COPY file:f30bcb89ff6df7709069d6cc97353d72cdbbebc6530d8d350cbb3ae4dad79129 in ./scripts/ 
# Fri, 17 Nov 2023 00:46:10 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Fri, 17 Nov 2023 00:46:10 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:4060ece20d7ac783f52cbe28a35fd5b06f90f7b4d773bae0d956024e85ff35b6`  
		Last Modified: Mon, 07 Aug 2023 19:39:59 GMT  
		Size: 3.3 MB (3258290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778a29448c85f5349db5c2a8c91e09bb24415f8c010133b0976a97ae37a40256`  
		Last Modified: Fri, 17 Nov 2023 00:46:20 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbe65f838346d33f66aab8d53809a78314c0e63cafb944226af3d5b9e1acd46`  
		Last Modified: Fri, 17 Nov 2023 00:46:21 GMT  
		Size: 3.1 MB (3135693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1044c67968016b714c1417c534fae5525be432f8be37e1aa22528fc52937a96`  
		Last Modified: Fri, 17 Nov 2023 00:46:22 GMT  
		Size: 11.6 MB (11616090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f867e3dbd8ae6a6a2799e4e63e5eac1eb529cd7996efac37386069f76071d5e`  
		Last Modified: Fri, 17 Nov 2023 00:46:20 GMT  
		Size: 1.9 KB (1950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8332e40d2e076a34ba7e23d9aa4f6fb509a4396302ddd7c197fa95fe09a145`  
		Last Modified: Fri, 17 Nov 2023 00:46:20 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
