## `eggdrop:develop`

```console
$ docker pull eggdrop@sha256:734121cfa76d658606747c1f5257fb8b96859ae35a987b40ab348639b32ad7bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:develop` - linux; amd64

```console
$ docker pull eggdrop@sha256:bc541fc728b554e4f7640cbdb9a68229aaac76d45b1aa6730ad08d7f32df484b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16124690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84396e5cb68862bf935730f66e5c1f08a3dcc09477841b3bdfe3e3d5a3f107f1`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:54:57 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 29 Mar 2023 19:54:58 GMT
RUN adduser -S eggdrop
# Wed, 29 Mar 2023 19:54:59 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 29 Mar 2023 19:54:59 GMT
ENV EGGDROP_SHA256=cc7936ee427959081651319119ac0b8f3581a18d7be7b20f71023954f1f69a91
# Wed, 29 Mar 2023 19:54:59 GMT
ENV EGGDROP_COMMIT=26ecf0921ee84c5bf61cb31014a75f02670b1af4
# Wed, 29 Mar 2023 19:55:00 GMT
RUN apk --update add --no-cache bash openssl
# Wed, 29 Mar 2023 19:58:37 GMT
RUN apk --update add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.13-src.tar.gz" -O tcl8.6.13-src.tar.gz   && tar -zxf tcl8.6.13-src.tar.gz   && ( cd tcl8.6.13     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm -rf tcl8.6.13-src.tar.gz   && rm -rf tcl8.6.13   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 29 Mar 2023 19:58:37 GMT
ENV NICK=
# Wed, 29 Mar 2023 19:58:37 GMT
ENV SERVER=
# Wed, 29 Mar 2023 19:58:37 GMT
ENV LISTEN=3333
# Wed, 29 Mar 2023 19:58:37 GMT
ENV OWNER=
# Wed, 29 Mar 2023 19:58:37 GMT
ENV USERFILE=eggdrop.user
# Wed, 29 Mar 2023 19:58:37 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 29 Mar 2023 19:58:37 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 29 Mar 2023 19:58:37 GMT
EXPOSE 3333
# Wed, 29 Mar 2023 19:58:38 GMT
COPY file:35e05bb72116a1848ec779e3fbc4ea6bbcd95ceb11059751f608c8543e18cde7 in /home/eggdrop/eggdrop 
# Wed, 29 Mar 2023 19:58:38 GMT
COPY file:f30bcb89ff6df7709069d6cc97353d72cdbbebc6530d8d350cbb3ae4dad79129 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 29 Mar 2023 19:58:38 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 29 Mar 2023 19:58:38 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448baa775d700b6d963b98900648a2a828a6e33dc23c5b146e833095c826d3bf`  
		Last Modified: Wed, 29 Mar 2023 20:03:08 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1edddd715dda5d8ca68ed2c72ad665f4ba9a79f3b5d7a3e190d45d2e5cec66a3`  
		Last Modified: Wed, 29 Mar 2023 20:03:06 GMT  
		Size: 11.0 KB (10979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d8f0c91f7f35c261be4b320d49652a14b869a7ea0ddc550b062742266c2779d`  
		Last Modified: Wed, 29 Mar 2023 20:03:06 GMT  
		Size: 1.2 MB (1202021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7296b3a61c4009b463590722a0e6080646f28e9e8f81c371a26cb41fc174bebe`  
		Last Modified: Wed, 29 Mar 2023 20:03:07 GMT  
		Size: 11.5 MB (11532897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a5973215293aa56051e3413de88292cd6608fe8809b7eb519bdd500bc4974f`  
		Last Modified: Wed, 29 Mar 2023 20:03:06 GMT  
		Size: 1.9 KB (1894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641588a22b8e55ee2967e817b9dfaddea36bafe614336433770a692aaa136ca6`  
		Last Modified: Wed, 29 Mar 2023 20:03:06 GMT  
		Size: 1.1 KB (1061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:b04c9ee90ae434c47a92e072bbe5b57531dbaa037afceaf1c681c13004a76b42
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15727050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c20287fe40eb276e9686ef4bea510b90ebafc1975f35e844d5f9022befbd0b`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:25 GMT
ADD file:07e668ef139dce7f076143a30b89ff57885c8539d8b5764ac1bd5277d9936702 in / 
# Wed, 14 Jun 2023 18:49:25 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 19:46:33 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 14 Jun 2023 19:46:34 GMT
RUN adduser -S eggdrop
# Wed, 14 Jun 2023 19:46:36 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 14 Jun 2023 19:46:36 GMT
ENV EGGDROP_SHA256=cc7936ee427959081651319119ac0b8f3581a18d7be7b20f71023954f1f69a91
# Wed, 14 Jun 2023 19:46:37 GMT
ENV EGGDROP_COMMIT=26ecf0921ee84c5bf61cb31014a75f02670b1af4
# Wed, 14 Jun 2023 19:46:38 GMT
RUN apk --update add --no-cache bash openssl
# Wed, 14 Jun 2023 19:50:44 GMT
RUN apk --update add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.13-src.tar.gz" -O tcl8.6.13-src.tar.gz   && tar -zxf tcl8.6.13-src.tar.gz   && ( cd tcl8.6.13     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm -rf tcl8.6.13-src.tar.gz   && rm -rf tcl8.6.13   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 14 Jun 2023 19:50:44 GMT
ENV NICK=
# Wed, 14 Jun 2023 19:50:45 GMT
ENV SERVER=
# Wed, 14 Jun 2023 19:50:45 GMT
ENV LISTEN=3333
# Wed, 14 Jun 2023 19:50:45 GMT
ENV OWNER=
# Wed, 14 Jun 2023 19:50:45 GMT
ENV USERFILE=eggdrop.user
# Wed, 14 Jun 2023 19:50:45 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 14 Jun 2023 19:50:45 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 14 Jun 2023 19:50:45 GMT
EXPOSE 3333
# Wed, 14 Jun 2023 19:50:45 GMT
COPY file:35e05bb72116a1848ec779e3fbc4ea6bbcd95ceb11059751f608c8543e18cde7 in /home/eggdrop/eggdrop 
# Wed, 14 Jun 2023 19:50:45 GMT
COPY file:f30bcb89ff6df7709069d6cc97353d72cdbbebc6530d8d350cbb3ae4dad79129 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 14 Jun 2023 19:50:45 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 14 Jun 2023 19:50:45 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:33ec62e98ceea71d24212ee03e239c2d5538dbe7c98f41c42e8b2693fedf58fb`  
		Last Modified: Wed, 14 Jun 2023 18:50:00 GMT  
		Size: 3.1 MB (3110916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da662cf081eacecc880868556d58fefa681f5a85748f715fa018059fc3610b9`  
		Last Modified: Wed, 14 Jun 2023 19:56:28 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1adc81653025f97685e7c96ba9145ecf37d5eb688af5653e202542ce7aa0af4`  
		Last Modified: Wed, 14 Jun 2023 19:56:26 GMT  
		Size: 11.1 KB (11135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f93b4e51f49c1a11557946eba1189df73b55efac200f2f9fdfcf88c4a2ccc789`  
		Last Modified: Wed, 14 Jun 2023 19:56:27 GMT  
		Size: 1.2 MB (1187432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b510499214f86b56fc84b2e8fce2d41a3c2ac6a01d3a339c5b6502e92f3968e8`  
		Last Modified: Wed, 14 Jun 2023 19:56:29 GMT  
		Size: 11.4 MB (11413335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6856ec7405ef9cab9d83cb843abb5b9880819c47362f0abd65c2adb821c61d33`  
		Last Modified: Wed, 14 Jun 2023 19:56:26 GMT  
		Size: 1.9 KB (1896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6058d001e9e054632a5c35775eaef1dc3e93a2b93e697f7d21e2d49ff024f6d0`  
		Last Modified: Wed, 14 Jun 2023 19:56:26 GMT  
		Size: 1.1 KB (1062 bytes)  
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
