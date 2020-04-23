## `eggdrop:develop`

```console
$ docker pull eggdrop@sha256:6e80af32e234a1a2ced55d590357a7e1d77d2b08d8d52c7a133bb6bc3efef0a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:develop` - linux; amd64

```console
$ docker pull eggdrop@sha256:7fc7146740ac23e356324f06c9d6002e06de60bf22cc4224a1d473b1e382faf5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.2 MB (13161878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03a4ededa2642b05e7e4f04aefbab25030c5a3d703400cbfb15e11ea0ef12f9f`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 22:01:51 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Mon, 23 Mar 2020 22:01:52 GMT
RUN adduser -S eggdrop
# Mon, 23 Mar 2020 22:01:54 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 23 Mar 2020 22:01:55 GMT
ENV EGGDROP_SHA256=12f560ad31e27f1ad631964f6d4ca43e97de6b11c35d4b733a44d21216d83bb4
# Mon, 23 Mar 2020 22:01:55 GMT
ENV EGGDROP_COMMIT=7a490c534fd53af99cbf33a85d907785e9156629
# Mon, 23 Mar 2020 22:01:58 GMT
RUN apk --update add --no-cache tcl bash openssl
# Mon, 23 Mar 2020 22:03:40 GMT
RUN apk --update add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256  develop.tar.gz" | sha256sum -c -   && tar -zxvf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 23 Mar 2020 22:03:41 GMT
ENV NICK=
# Mon, 23 Mar 2020 22:03:41 GMT
ENV SERVER=
# Mon, 23 Mar 2020 22:03:41 GMT
ENV LISTEN=3333
# Mon, 23 Mar 2020 22:03:42 GMT
ENV OWNER=
# Mon, 23 Mar 2020 22:03:42 GMT
ENV USERFILE=eggdrop.user
# Mon, 23 Mar 2020 22:03:42 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 23 Mar 2020 22:03:43 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 23 Mar 2020 22:03:43 GMT
EXPOSE 3333
# Mon, 23 Mar 2020 22:03:44 GMT
COPY file:4b2e5310f8e2b48c1ffa7bba797207637a35204a73634e98dc622889d320f394 in /home/eggdrop/eggdrop 
# Mon, 23 Mar 2020 22:03:44 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 23 Mar 2020 22:03:45 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 23 Mar 2020 22:03:45 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de90ac254f3b2092e08d0d1a27fade104236143c7429ad4bfd7a17858c302031`  
		Last Modified: Mon, 23 Mar 2020 22:05:43 GMT  
		Size: 1.2 KB (1236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7989bd96822c15f6ae1d0789c29950de5717ef922d3f3f8e284011e9e169c4`  
		Last Modified: Mon, 23 Mar 2020 22:05:41 GMT  
		Size: 9.6 KB (9581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c6f695262d96126f5d8ace179315acdee7e373a1758730524daad3dc571e81`  
		Last Modified: Mon, 23 Mar 2020 22:05:42 GMT  
		Size: 2.7 MB (2684257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660b0b8f894961a00dd343f973f8e3e029cf6cf07e6008a1ab3b99939369b623`  
		Last Modified: Mon, 23 Mar 2020 22:05:43 GMT  
		Size: 7.7 MB (7660959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaeb4a05350a979e38a4258d792a75fbf628d49449be1c3786a6839c4a647f91`  
		Last Modified: Mon, 23 Mar 2020 22:05:41 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbbdfc077c3e48e443051bfe7f83a6d15187d16766b62278f09cdb63b71a8dac`  
		Last Modified: Mon, 23 Mar 2020 22:05:41 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:66b70820b405a82c2be740969af6e10e6acda0dcd663f53d38189df4fdbba93c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.8 MB (12845127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb459cffc9df6a6ffa5858548420eccbb14b254d2b8bc988e69d57244d7d0796`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 17:36:48 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 23 Apr 2020 17:36:52 GMT
RUN adduser -S eggdrop
# Thu, 23 Apr 2020 17:36:54 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 23 Apr 2020 17:36:55 GMT
ENV EGGDROP_SHA256=12f560ad31e27f1ad631964f6d4ca43e97de6b11c35d4b733a44d21216d83bb4
# Thu, 23 Apr 2020 17:36:56 GMT
ENV EGGDROP_COMMIT=7a490c534fd53af99cbf33a85d907785e9156629
# Thu, 23 Apr 2020 17:37:03 GMT
RUN apk --update add --no-cache tcl bash openssl
# Thu, 23 Apr 2020 17:39:04 GMT
RUN apk --update add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256  develop.tar.gz" | sha256sum -c -   && tar -zxvf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 23 Apr 2020 17:39:05 GMT
ENV NICK=
# Thu, 23 Apr 2020 17:39:06 GMT
ENV SERVER=
# Thu, 23 Apr 2020 17:39:07 GMT
ENV LISTEN=3333
# Thu, 23 Apr 2020 17:39:08 GMT
ENV OWNER=
# Thu, 23 Apr 2020 17:39:08 GMT
ENV USERFILE=eggdrop.user
# Thu, 23 Apr 2020 17:39:09 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 23 Apr 2020 17:39:10 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 23 Apr 2020 17:39:10 GMT
EXPOSE 3333
# Thu, 23 Apr 2020 17:39:11 GMT
COPY file:4b2e5310f8e2b48c1ffa7bba797207637a35204a73634e98dc622889d320f394 in /home/eggdrop/eggdrop 
# Thu, 23 Apr 2020 17:39:12 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 23 Apr 2020 17:39:12 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 23 Apr 2020 17:39:13 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f412a5980f526ade995939566f7c342b9adb4c13754922fed8d1798066f9eed`  
		Last Modified: Thu, 23 Apr 2020 17:39:27 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f404049eca1aec0b894cf78c6e968dd2065753284309b55be17f3291c31ad065`  
		Last Modified: Thu, 23 Apr 2020 17:39:24 GMT  
		Size: 9.4 KB (9390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59742158857b1dd535ac41399f7d4394181e53384e9d232920dbd3ea76141c65`  
		Last Modified: Thu, 23 Apr 2020 17:39:25 GMT  
		Size: 2.6 MB (2608162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576b568885b56ef30dc69ec15ad3d84230b828a17b49595a616e12d97f400426`  
		Last Modified: Thu, 23 Apr 2020 17:39:26 GMT  
		Size: 7.6 MB (7603793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0bec210903ad7e7f55610ab22068f322a6c530668ca880b62d975730bbb974`  
		Last Modified: Thu, 23 Apr 2020 17:39:24 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7c734405bebe7061ba5895931c94d0119a538922bfbcc62024ee7abbf21d18`  
		Last Modified: Thu, 23 Apr 2020 17:39:25 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:a7303960fe0cbc56bad1453aeede82f0eb45d110346f51fcc0bcac0383ced13f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13141692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3713e34c0e691a1f9d079aa4e12d1f1c8fd3ba6454881205cb40219abd179e2`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Mon, 23 Mar 2020 21:39:52 GMT
ADD file:746a5c3838a898d6acf7877552ff13d1ab40d0036ace7a662e7c747018315ddb in / 
# Mon, 23 Mar 2020 21:39:53 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 23:21:10 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Mon, 23 Mar 2020 23:21:12 GMT
RUN adduser -S eggdrop
# Mon, 23 Mar 2020 23:21:14 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 23 Mar 2020 23:21:15 GMT
ENV EGGDROP_SHA256=12f560ad31e27f1ad631964f6d4ca43e97de6b11c35d4b733a44d21216d83bb4
# Mon, 23 Mar 2020 23:21:15 GMT
ENV EGGDROP_COMMIT=7a490c534fd53af99cbf33a85d907785e9156629
# Mon, 23 Mar 2020 23:21:18 GMT
RUN apk --update add --no-cache tcl bash openssl
# Mon, 23 Mar 2020 23:23:11 GMT
RUN apk --update add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256  develop.tar.gz" | sha256sum -c -   && tar -zxvf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Mon, 23 Mar 2020 23:23:12 GMT
ENV NICK=
# Mon, 23 Mar 2020 23:23:13 GMT
ENV SERVER=
# Mon, 23 Mar 2020 23:23:15 GMT
ENV LISTEN=3333
# Mon, 23 Mar 2020 23:23:16 GMT
ENV OWNER=
# Mon, 23 Mar 2020 23:23:17 GMT
ENV USERFILE=eggdrop.user
# Mon, 23 Mar 2020 23:23:18 GMT
ENV CHANFILE=eggdrop.chan
# Mon, 23 Mar 2020 23:23:20 GMT
WORKDIR /home/eggdrop/eggdrop
# Mon, 23 Mar 2020 23:23:21 GMT
EXPOSE 3333
# Mon, 23 Mar 2020 23:23:22 GMT
COPY file:4b2e5310f8e2b48c1ffa7bba797207637a35204a73634e98dc622889d320f394 in /home/eggdrop/eggdrop 
# Mon, 23 Mar 2020 23:23:23 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Mon, 23 Mar 2020 23:23:24 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Mon, 23 Mar 2020 23:23:26 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:8a0637ca1ac98db4cf29f7632449c92801adc80cf0da2cd9c9e39882ce466561`  
		Last Modified: Mon, 23 Mar 2020 21:40:19 GMT  
		Size: 2.7 MB (2723139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b63c1a6e13b1a71398150ac595bcf7f9da6e35406fb414527335ac85fa4a5b`  
		Last Modified: Mon, 23 Mar 2020 23:23:47 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585c313e804e3c02c867edec0ce1532cc51d93d8e0cd199e5e872ffdc3299b14`  
		Last Modified: Mon, 23 Mar 2020 23:23:46 GMT  
		Size: 9.5 KB (9507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c895227bac8b1f2f8bf3356f31965f1c810cbb69e6068ec3b7b29d395051b59`  
		Last Modified: Mon, 23 Mar 2020 23:23:46 GMT  
		Size: 2.7 MB (2722233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14a5225693f9d1dfb74d4c6dbf7473413861f2ce45081fb5b92ca9ff8a0dca1`  
		Last Modified: Mon, 23 Mar 2020 23:23:47 GMT  
		Size: 7.7 MB (7682965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f90977b178413a0ea4f9490ad81aba20c3e84537be9ae22e6940ea0d9eef07`  
		Last Modified: Mon, 23 Mar 2020 23:23:45 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df0e30f597c3c6f85ba179f950cbc78c89fb0fbc5267564132b4d3769c4fa22`  
		Last Modified: Mon, 23 Mar 2020 23:23:46 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
