## `eggdrop:develop`

```console
$ docker pull eggdrop@sha256:ad8499cf0120784c4a57db2b003e8c0cd71db3a8e2b16f799c3abb7f44cb7045
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:develop` - linux; amd64

```console
$ docker pull eggdrop@sha256:beb13e638658e3b00b22b8d49f0f694ce40372c332caacd0b4fb899805e2f6b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16127511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:403fd9a31d4e69ba0897411e2818757e18a40f6645270de9d08560940d87a930`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 04:38:29 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 15 Jun 2023 04:38:29 GMT
RUN adduser -S eggdrop
# Thu, 15 Jun 2023 04:38:30 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 15 Jun 2023 04:38:30 GMT
ENV EGGDROP_SHA256=cc7936ee427959081651319119ac0b8f3581a18d7be7b20f71023954f1f69a91
# Thu, 15 Jun 2023 04:38:31 GMT
ENV EGGDROP_COMMIT=26ecf0921ee84c5bf61cb31014a75f02670b1af4
# Thu, 15 Jun 2023 04:38:32 GMT
RUN apk --update add --no-cache bash openssl
# Thu, 15 Jun 2023 04:42:12 GMT
RUN apk --update add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.13-src.tar.gz" -O tcl8.6.13-src.tar.gz   && tar -zxf tcl8.6.13-src.tar.gz   && ( cd tcl8.6.13     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm -rf tcl8.6.13-src.tar.gz   && rm -rf tcl8.6.13   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 15 Jun 2023 04:42:12 GMT
ENV NICK=
# Thu, 15 Jun 2023 04:42:13 GMT
ENV SERVER=
# Thu, 15 Jun 2023 04:42:13 GMT
ENV LISTEN=3333
# Thu, 15 Jun 2023 04:42:13 GMT
ENV OWNER=
# Thu, 15 Jun 2023 04:42:13 GMT
ENV USERFILE=eggdrop.user
# Thu, 15 Jun 2023 04:42:13 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 15 Jun 2023 04:42:13 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 15 Jun 2023 04:42:13 GMT
EXPOSE 3333
# Thu, 15 Jun 2023 04:42:13 GMT
COPY file:35e05bb72116a1848ec779e3fbc4ea6bbcd95ceb11059751f608c8543e18cde7 in /home/eggdrop/eggdrop 
# Thu, 15 Jun 2023 04:42:13 GMT
COPY file:f30bcb89ff6df7709069d6cc97353d72cdbbebc6530d8d350cbb3ae4dad79129 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 15 Jun 2023 04:42:13 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 15 Jun 2023 04:42:13 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714c670ef22550a4a3ad9dd2eb8e0a56039cbdfb6748dc13d83eb3b347d0d5bd`  
		Last Modified: Thu, 15 Jun 2023 04:46:40 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc28894795b7ded44f6fc10e49e88ed71e71a3de7cda2b74c9818668bde3d03`  
		Last Modified: Thu, 15 Jun 2023 04:46:38 GMT  
		Size: 11.0 KB (10987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de551f5b9224829504860f0ebd32c88971602800fc8ff16e3ef56e552269cc80`  
		Last Modified: Thu, 15 Jun 2023 04:46:38 GMT  
		Size: 1.2 MB (1203427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead754afd421d8b5d6ad963afbbd03640b17040e38b7fcc20fbb779065c7cad0`  
		Last Modified: Thu, 15 Jun 2023 04:46:40 GMT  
		Size: 11.5 MB (11534163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55ab9123a62b7db38c6d20c95a5fc287239ae4a695511c89fcbbe1c4e9db34f2`  
		Last Modified: Thu, 15 Jun 2023 04:46:38 GMT  
		Size: 1.9 KB (1891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2687eb09fc414be6f8254fa2597136a4c68d65d0f62b6a8f57ed59f74bd4f9b`  
		Last Modified: Thu, 15 Jun 2023 04:46:38 GMT  
		Size: 1.1 KB (1057 bytes)  
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
$ docker pull eggdrop@sha256:d6ee40eddcd6b4a135621b7b30c03b37126ea9caa8a0351ddabc3d3355e48154
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16104053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:100ca47c5d29b68946c3c6b138af46476c2bb77c08d9c9829d9b71642a7cda37`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:04 GMT
ADD file:6f6c919dc1fe5a56c2664a26a702d77203039cdd4c91e39da57063ea5d3f3094 in / 
# Wed, 14 Jun 2023 20:49:04 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 22:47:42 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 14 Jun 2023 22:47:42 GMT
RUN adduser -S eggdrop
# Wed, 14 Jun 2023 22:47:44 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 14 Jun 2023 22:47:44 GMT
ENV EGGDROP_SHA256=cc7936ee427959081651319119ac0b8f3581a18d7be7b20f71023954f1f69a91
# Wed, 14 Jun 2023 22:47:44 GMT
ENV EGGDROP_COMMIT=26ecf0921ee84c5bf61cb31014a75f02670b1af4
# Wed, 14 Jun 2023 22:47:45 GMT
RUN apk --update add --no-cache bash openssl
# Wed, 14 Jun 2023 22:51:02 GMT
RUN apk --update add --no-cache --virtual egg-deps wget ca-certificates make tar gnupg build-base openssl-dev   && wget "https://prdownloads.sourceforge.net/tcl/tcl8.6.13-src.tar.gz" -O tcl8.6.13-src.tar.gz   && tar -zxf tcl8.6.13-src.tar.gz   && ( cd tcl8.6.13     && sed -i "/define TCL_UTF_MAX/c\#define TCL_UTF_MAX 6" generic/tcl.h     && cd unix     && ./configure     && make     && make install )   && rm -rf tcl8.6.13-src.tar.gz   && rm -rf tcl8.6.13   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256 *develop.tar.gz" | sha256sum -c -   && tar -zxf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 14 Jun 2023 22:51:02 GMT
ENV NICK=
# Wed, 14 Jun 2023 22:51:02 GMT
ENV SERVER=
# Wed, 14 Jun 2023 22:51:02 GMT
ENV LISTEN=3333
# Wed, 14 Jun 2023 22:51:02 GMT
ENV OWNER=
# Wed, 14 Jun 2023 22:51:02 GMT
ENV USERFILE=eggdrop.user
# Wed, 14 Jun 2023 22:51:02 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 14 Jun 2023 22:51:02 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 14 Jun 2023 22:51:03 GMT
EXPOSE 3333
# Wed, 14 Jun 2023 22:51:03 GMT
COPY file:35e05bb72116a1848ec779e3fbc4ea6bbcd95ceb11059751f608c8543e18cde7 in /home/eggdrop/eggdrop 
# Wed, 14 Jun 2023 22:51:03 GMT
COPY file:f30bcb89ff6df7709069d6cc97353d72cdbbebc6530d8d350cbb3ae4dad79129 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 14 Jun 2023 22:51:03 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 14 Jun 2023 22:51:03 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:edb6bdbacee93be93e930669f43e2e922c8594676aa342a70e2221361fd1914d`  
		Last Modified: Wed, 14 Jun 2023 20:49:35 GMT  
		Size: 3.3 MB (3261139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab556bb27c3eeadbcc437904e4d024f7ab53548eb269e2f05babbd5d673b7f06`  
		Last Modified: Wed, 14 Jun 2023 22:55:21 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:821fe5f3cdc578d1e7bf2c18f3185bd991b368062f1a7c6b6edf42d1d1bd2c9c`  
		Last Modified: Wed, 14 Jun 2023 22:55:19 GMT  
		Size: 11.2 KB (11189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c154146375088dd23f935a6db1f78af30a7913b4a60903db68641c8822f425bc`  
		Last Modified: Wed, 14 Jun 2023 22:55:19 GMT  
		Size: 1.2 MB (1234460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b9bf5d321b4c83ed35be7d9f12decc16635c4dd88fb9aa9a6192ac3b26b237`  
		Last Modified: Wed, 14 Jun 2023 22:55:20 GMT  
		Size: 11.6 MB (11593040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:821f8b68fcae9339ef33904560aade133f4b38dae0fa947938aa1b094651f365`  
		Last Modified: Wed, 14 Jun 2023 22:55:19 GMT  
		Size: 1.9 KB (1891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae53839769fce95bc4bcf305e8d8bbf34e1820445b05c558cc53dd2dafd53aff`  
		Last Modified: Wed, 14 Jun 2023 22:55:19 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
