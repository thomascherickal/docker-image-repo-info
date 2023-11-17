## `eggdrop:develop`

```console
$ docker pull eggdrop@sha256:afe2edc84220f5db578e0dcc1349e624e36d9080a5343854dd9dcadd7ecf2a67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:develop` - linux; amd64

```console
$ docker pull eggdrop@sha256:9ec6b149a789433e2df240dce0dc83a36c33c82d50361683f7b1d0145331342a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.2 MB (18181286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4df521af73130bbe77b03bd8ecc6b8a34b79233f59eb491c1eadc2f4a50df0a`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:17:09 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Sat, 21 Oct 2023 00:17:10 GMT
RUN adduser -S eggdrop
# Sat, 21 Oct 2023 00:17:11 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 21 Oct 2023 00:17:11 GMT
ENV EGGDROP_SHA256=cc7936ee427959081651319119ac0b8f3581a18d7be7b20f71023954f1f69a91
# Sat, 21 Oct 2023 00:17:11 GMT
ENV EGGDROP_COMMIT=26ecf0921ee84c5bf61cb31014a75f02670b1af4
# Sat, 21 Oct 2023 00:17:12 GMT
RUN apk --update add --no-cache bash openssl
# Sat, 21 Oct 2023 00:20:47 GMT
RUN apk --update add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.13-src.tar.gz" -O tcl8.6.13-src.tar.gz   && tar -zxf tcl8.6.13-src.tar.gz   && ( cd tcl8.6.13     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm -rf tcl8.6.13-src.tar.gz   && rm -rf tcl8.6.13   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Sat, 21 Oct 2023 00:20:47 GMT
ENV NICK=
# Sat, 21 Oct 2023 00:20:47 GMT
ENV SERVER=
# Sat, 21 Oct 2023 00:20:47 GMT
ENV LISTEN=3333
# Sat, 21 Oct 2023 00:20:48 GMT
ENV OWNER=
# Sat, 21 Oct 2023 00:20:48 GMT
ENV USERFILE=eggdrop.user
# Sat, 21 Oct 2023 00:20:48 GMT
ENV CHANFILE=eggdrop.chan
# Sat, 21 Oct 2023 00:20:48 GMT
WORKDIR /home/eggdrop/eggdrop
# Sat, 21 Oct 2023 00:20:48 GMT
EXPOSE 3333
# Sat, 21 Oct 2023 00:20:48 GMT
COPY file:35e05bb72116a1848ec779e3fbc4ea6bbcd95ceb11059751f608c8543e18cde7 in /home/eggdrop/eggdrop 
# Sat, 21 Oct 2023 00:20:48 GMT
COPY file:f30bcb89ff6df7709069d6cc97353d72cdbbebc6530d8d350cbb3ae4dad79129 in /home/eggdrop/eggdrop/scripts/ 
# Sat, 21 Oct 2023 00:20:48 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Sat, 21 Oct 2023 00:20:48 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5097e7c90940c1ad08f4c14384b6e2b7bab2641e3962c1d08ea52eed9ae3cd5a`  
		Last Modified: Sat, 21 Oct 2023 00:25:21 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6848297e98706c32911ba7521bbbcb939e30b344e80d82a4c23ae786c4bce2c`  
		Last Modified: Sat, 21 Oct 2023 00:25:19 GMT  
		Size: 11.0 KB (10989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a7878a3e855d542a57210de1c56489094335eee11c07130b0fb1c43d9382d1`  
		Last Modified: Sat, 21 Oct 2023 00:25:19 GMT  
		Size: 3.3 MB (3252168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c554af8b3fe3416653bd54e0be76715af3815378bc526f99d99db471dcc56eab`  
		Last Modified: Sat, 21 Oct 2023 00:25:21 GMT  
		Size: 11.5 MB (11535291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcad910f3e97b3929931557c9fc1dd692de3dc7a35634dae4b16a1dcd47ad663`  
		Last Modified: Sat, 21 Oct 2023 00:25:19 GMT  
		Size: 1.9 KB (1892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd80a7788f9c59b9fbbfe008475855d8ea16bf7def77b49ffcd90b07b9de35ca`  
		Last Modified: Sat, 21 Oct 2023 00:25:19 GMT  
		Size: 1.1 KB (1060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:7ec24e9f4e60c69e368d49d2d118598683c4ce03b7f6b396f9764045daa8db22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.5 MB (17464976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c23cbe7f13a59d0657331d9ef3c321afc9e4a3ee006220b1642ad98dd1d19a6`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:17 GMT
ADD file:cb3f59b0f701cb6ef552e7f8ada1707cf82747c95b69759924061ff9ac6dbe72 in / 
# Mon, 07 Aug 2023 19:49:18 GMT
CMD ["/bin/sh"]
# Fri, 17 Nov 2023 00:49:16 GMT
LABEL org.opencontainers.image.authors=Geo Van O <geo@eggheads.org> org.opencontainers.image.url=https://www.eggheads.org
# Fri, 17 Nov 2023 00:49:17 GMT
RUN addgroup -S -g 3333 eggdrop     && adduser -S -u 3333 eggdrop eggdrop
# Fri, 17 Nov 2023 00:49:18 GMT
RUN apk add --no-cache 'su-exec>=0.2' bash openssl
# Fri, 17 Nov 2023 00:49:18 GMT
ENV EGGDROP_SHA256=a155625d2ac3a0673e69c9d0149293910583c1623cd1f90f38ad2bcba7b2b766
# Fri, 17 Nov 2023 00:49:19 GMT
ENV EGGDROP_COMMIT=322bddbd102d58cdb00864a3a335b086beaf042c
# Fri, 17 Nov 2023 00:51:31 GMT
RUN apk add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.13-src.tar.gz" -O tcl8.6.13-src.tar.gz --progress=dot:giga   && tar -zxf tcl8.6.13-src.tar.gz   && ( cd tcl8.6.13     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && nproc="$(nproc)"     && make -j"$nproc"     && make install )   && rm -rf tcl8.6.13-src.tar.gz   && rm -rf tcl8.6.13   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && nproc="$(nproc)"     && make -j"$nproc"     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del --no-network egg-deps
# Fri, 17 Nov 2023 00:51:31 GMT
ENV NICK=
# Fri, 17 Nov 2023 00:51:31 GMT
ENV SERVER=
# Fri, 17 Nov 2023 00:51:31 GMT
ENV LISTEN=3333
# Fri, 17 Nov 2023 00:51:31 GMT
ENV USERFILE=eggdrop.user
# Fri, 17 Nov 2023 00:51:32 GMT
ENV CHANFILE=eggdrop.chan
# Fri, 17 Nov 2023 00:51:32 GMT
WORKDIR /home/eggdrop/eggdrop
# Fri, 17 Nov 2023 00:51:32 GMT
EXPOSE 3333
# Fri, 17 Nov 2023 00:51:32 GMT
COPY file:15b1df22891b2d819093301ed85a114b9e76e06ecf7eba8f403edb7908e4aebf in ./ 
# Fri, 17 Nov 2023 00:51:32 GMT
COPY file:f30bcb89ff6df7709069d6cc97353d72cdbbebc6530d8d350cbb3ae4dad79129 in ./scripts/ 
# Fri, 17 Nov 2023 00:51:32 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Fri, 17 Nov 2023 00:51:32 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:342323bc858ed9706f7953ab06cbf6785b678c55ef2317577af748533d11165b`  
		Last Modified: Mon, 07 Aug 2023 19:49:53 GMT  
		Size: 3.1 MB (3112450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:335fc6f78cbd562d8f9766b3257ac3d9b37fa428d12b64f5070920d39939eae0`  
		Last Modified: Fri, 17 Nov 2023 00:51:47 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:861d3f8e3ba7e46d7b9ed9155c9a3fe18596e62335e22629aeef6ca4ba5e9021`  
		Last Modified: Fri, 17 Nov 2023 00:51:47 GMT  
		Size: 2.9 MB (2910069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a088eea7dc41afcb28fdefb3e171a8cd00c1fb63027a8a0a94ebb8d13e7dafc`  
		Last Modified: Fri, 17 Nov 2023 00:51:49 GMT  
		Size: 11.4 MB (11438170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576576d87dc427bcb07cbd63374bca0e5cae39bea4b2c10322dc45770ea62014`  
		Last Modified: Fri, 17 Nov 2023 00:51:47 GMT  
		Size: 2.0 KB (1951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98259cceccb04b799758c7a457ef8f75825469cd4925e40995c3d32bca9b45b`  
		Last Modified: Fri, 17 Nov 2023 00:51:47 GMT  
		Size: 1.1 KB (1058 bytes)  
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
