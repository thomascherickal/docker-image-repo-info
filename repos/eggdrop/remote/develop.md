## `eggdrop:develop`

```console
$ docker pull eggdrop@sha256:f4a264126262bf08457dbb694b382e82f3904f4d7d4217b049f83ec09fef0769
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:develop` - linux; amd64

```console
$ docker pull eggdrop@sha256:f4dda8dbfc8340afdb126c0060918804fce7479c781fea005f3bb8cb90a3e086
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16124763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ae7b6f7479c5d54b5d4f907ec43ab5feb20c95f593915f87378b72b94a6efd4`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 20:24:51 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Mon, 13 Mar 2023 20:24:52 GMT
RUN adduser -S eggdrop
# Mon, 13 Mar 2023 20:24:53 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 13 Mar 2023 20:24:53 GMT
ENV EGGDROP_SHA256=cc7936ee427959081651319119ac0b8f3581a18d7be7b20f71023954f1f69a91
# Mon, 13 Mar 2023 20:24:53 GMT
ENV EGGDROP_COMMIT=26ecf0921ee84c5bf61cb31014a75f02670b1af4
# Mon, 13 Mar 2023 20:24:54 GMT
RUN apk --update add --no-cache bash openssl
# Mon, 13 Mar 2023 20:28:32 GMT
RUN apk --update add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.13-src.tar.gz" -O tcl8.6.13-src.tar.gz   && tar -zxf tcl8.6.13-src.tar.gz   && ( cd tcl8.6.13     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm -rf tcl8.6.13-src.tar.gz   && rm -rf tcl8.6.13   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 13 Mar 2023 20:28:32 GMT
ENV NICK=
# Mon, 13 Mar 2023 20:28:32 GMT
ENV SERVER=
# Mon, 13 Mar 2023 20:28:32 GMT
ENV LISTEN=3333
# Mon, 13 Mar 2023 20:28:33 GMT
ENV OWNER=
# Mon, 13 Mar 2023 20:28:33 GMT
ENV USERFILE=eggdrop.user
# Mon, 13 Mar 2023 20:28:33 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 13 Mar 2023 20:28:33 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 13 Mar 2023 20:28:33 GMT
EXPOSE 3333
# Mon, 13 Mar 2023 20:28:33 GMT
COPY file:35e05bb72116a1848ec779e3fbc4ea6bbcd95ceb11059751f608c8543e18cde7 in /home/eggdrop/eggdrop 
# Mon, 13 Mar 2023 20:28:33 GMT
COPY file:f30bcb89ff6df7709069d6cc97353d72cdbbebc6530d8d350cbb3ae4dad79129 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 13 Mar 2023 20:28:33 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 13 Mar 2023 20:28:33 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9266924772c11264278e8f7e9f3f47dcee1457bf7675615f5ea055188cf85f16`  
		Last Modified: Mon, 13 Mar 2023 20:33:03 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1250f5956177bcd3a38a3665961d74a6441095a6631b42607cb3b1bdc8e53cd`  
		Last Modified: Mon, 13 Mar 2023 20:33:01 GMT  
		Size: 11.0 KB (10987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f57101f337e18f728b8805f2c9c720b9eb2e51fcae646a64f79663025dc1146`  
		Last Modified: Mon, 13 Mar 2023 20:33:01 GMT  
		Size: 1.2 MB (1202022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6cf3036a96c935256f63d8ddbd5c7f3ac6921566cef6753c6f06a3957765df1`  
		Last Modified: Mon, 13 Mar 2023 20:33:03 GMT  
		Size: 11.5 MB (11533076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc935cd2576555a7689ece02bcf0866b3f420389146b7f0db863abd0f5c87733`  
		Last Modified: Mon, 13 Mar 2023 20:33:01 GMT  
		Size: 1.9 KB (1895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32b2faffd8eedb0ba89d3d156d65a9712e4d488f2997630d6207476b6f075b38`  
		Last Modified: Mon, 13 Mar 2023 20:33:01 GMT  
		Size: 1.1 KB (1062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:63cc5fc1beb8311350e7a8e70df4a3fd64b4100eee5091b4811f10d88fb02815
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15724637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4117215b1d593900b6f4cab2d6da9e84cc85f106811899418b6bc5b326e820e`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:44 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Mon, 13 Mar 2023 16:12:44 GMT
CMD ["/bin/sh"]
# Tue, 14 Mar 2023 03:51:35 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Tue, 14 Mar 2023 03:51:35 GMT
RUN adduser -S eggdrop
# Tue, 14 Mar 2023 03:51:36 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 14 Mar 2023 03:51:36 GMT
ENV EGGDROP_SHA256=cc7936ee427959081651319119ac0b8f3581a18d7be7b20f71023954f1f69a91
# Tue, 14 Mar 2023 03:51:36 GMT
ENV EGGDROP_COMMIT=26ecf0921ee84c5bf61cb31014a75f02670b1af4
# Tue, 14 Mar 2023 03:51:37 GMT
RUN apk --update add --no-cache bash openssl
# Tue, 14 Mar 2023 03:55:26 GMT
RUN apk --update add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.13-src.tar.gz" -O tcl8.6.13-src.tar.gz   && tar -zxf tcl8.6.13-src.tar.gz   && ( cd tcl8.6.13     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm -rf tcl8.6.13-src.tar.gz   && rm -rf tcl8.6.13   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Tue, 14 Mar 2023 03:55:27 GMT
ENV NICK=
# Tue, 14 Mar 2023 03:55:27 GMT
ENV SERVER=
# Tue, 14 Mar 2023 03:55:27 GMT
ENV LISTEN=3333
# Tue, 14 Mar 2023 03:55:28 GMT
ENV OWNER=
# Tue, 14 Mar 2023 03:55:28 GMT
ENV USERFILE=eggdrop.user
# Tue, 14 Mar 2023 03:55:28 GMT
ENV CHANFILE=eggdrop.chan
# Tue, 14 Mar 2023 03:55:28 GMT
WORKDIR /home/eggdrop/eggdrop
# Tue, 14 Mar 2023 03:55:29 GMT
EXPOSE 3333
# Tue, 14 Mar 2023 03:55:29 GMT
COPY file:35e05bb72116a1848ec779e3fbc4ea6bbcd95ceb11059751f608c8543e18cde7 in /home/eggdrop/eggdrop 
# Tue, 14 Mar 2023 03:55:30 GMT
COPY file:f30bcb89ff6df7709069d6cc97353d72cdbbebc6530d8d350cbb3ae4dad79129 in /home/eggdrop/eggdrop/scripts/ 
# Tue, 14 Mar 2023 03:55:30 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Tue, 14 Mar 2023 03:55:30 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd87d9b3b4ff58c3588d6d208bced6615eaa5f74106a89e9f3c29f23a44bbd92`  
		Last Modified: Tue, 14 Mar 2023 04:00:29 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32a580d0f1caac5626e37402673d6cf802c43b381e2db2f3d8e85ac70f4ac05c`  
		Last Modified: Tue, 14 Mar 2023 04:00:26 GMT  
		Size: 11.1 KB (11131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75df0b575ab0b1b0b601757f305dbb61a8a82024c5813133584a89fe6bb50694`  
		Last Modified: Tue, 14 Mar 2023 04:00:27 GMT  
		Size: 1.2 MB (1186210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c86318a88b5c7630afa5c8955c9030bbf1d44b414351f6e815eae6170e16b34`  
		Last Modified: Tue, 14 Mar 2023 04:00:29 GMT  
		Size: 11.4 MB (11412173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6635be4ba7d82a268e18d18a9dec1acddf9cc697b2a32e09f4d2fffbf698f18`  
		Last Modified: Tue, 14 Mar 2023 04:00:26 GMT  
		Size: 1.9 KB (1897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf377a67ab80f0ae7aad5305b15e05830e1c1b77bce7028babb976eec8327fc5`  
		Last Modified: Tue, 14 Mar 2023 04:00:26 GMT  
		Size: 1.1 KB (1065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:02145b19b355da6bcb8d539238912b65ef4f4a01b951b517d35e46a28870fa83
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16105068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13cb4c99c02b85a5b5e2c27e6801a193c19803d1da9747a1e1936f5df194fbe4`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 17:58:38 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 29 Mar 2023 17:58:39 GMT
RUN adduser -S eggdrop
# Wed, 29 Mar 2023 17:58:40 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 29 Mar 2023 17:58:40 GMT
ENV EGGDROP_SHA256=cc7936ee427959081651319119ac0b8f3581a18d7be7b20f71023954f1f69a91
# Wed, 29 Mar 2023 17:58:40 GMT
ENV EGGDROP_COMMIT=26ecf0921ee84c5bf61cb31014a75f02670b1af4
# Wed, 29 Mar 2023 17:58:41 GMT
RUN apk --update add --no-cache bash openssl
# Wed, 29 Mar 2023 18:02:00 GMT
RUN apk --update add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.13-src.tar.gz" -O tcl8.6.13-src.tar.gz   && tar -zxf tcl8.6.13-src.tar.gz   && ( cd tcl8.6.13     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm -rf tcl8.6.13-src.tar.gz   && rm -rf tcl8.6.13   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 29 Mar 2023 18:02:00 GMT
ENV NICK=
# Wed, 29 Mar 2023 18:02:00 GMT
ENV SERVER=
# Wed, 29 Mar 2023 18:02:00 GMT
ENV LISTEN=3333
# Wed, 29 Mar 2023 18:02:00 GMT
ENV OWNER=
# Wed, 29 Mar 2023 18:02:00 GMT
ENV USERFILE=eggdrop.user
# Wed, 29 Mar 2023 18:02:01 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 29 Mar 2023 18:02:01 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 29 Mar 2023 18:02:01 GMT
EXPOSE 3333
# Wed, 29 Mar 2023 18:02:01 GMT
COPY file:35e05bb72116a1848ec779e3fbc4ea6bbcd95ceb11059751f608c8543e18cde7 in /home/eggdrop/eggdrop 
# Wed, 29 Mar 2023 18:02:01 GMT
COPY file:f30bcb89ff6df7709069d6cc97353d72cdbbebc6530d8d350cbb3ae4dad79129 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 29 Mar 2023 18:02:01 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 29 Mar 2023 18:02:01 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c91c2b5610b0ebf373765106488fc16d0eec5c20a499e88b30becdb08a9f9903`  
		Last Modified: Wed, 29 Mar 2023 18:06:17 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19ac67c8f11f17dc932ce797b534c6c348492ac2cbc8163ef410ecad15d3628`  
		Last Modified: Wed, 29 Mar 2023 18:06:16 GMT  
		Size: 11.2 KB (11184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473234a20c062f1e3b88a9cb43d551f41abf7f74a8da1e4fd7fb651f64430d82`  
		Last Modified: Wed, 29 Mar 2023 18:06:16 GMT  
		Size: 1.2 MB (1233181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3409786ba6676e4df657c0e9905cfbee6aeef0b9a035a348b451c9c87f29315e`  
		Last Modified: Wed, 29 Mar 2023 18:06:17 GMT  
		Size: 11.6 MB (11594624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9dcac42c924e970223b2dcccab46a8e2a2d918d55a704ad4bbb73a8591e7f05`  
		Last Modified: Wed, 29 Mar 2023 18:06:15 GMT  
		Size: 1.9 KB (1894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3615e205be5683b484cb4927e849a95683d5f4e92040bdc1805b5dc881620d`  
		Last Modified: Wed, 29 Mar 2023 18:06:15 GMT  
		Size: 1.1 KB (1060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
