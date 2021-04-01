## `eggdrop:develop`

```console
$ docker pull eggdrop@sha256:017a8ff63c4f783f563122e1707ac6fece322805611c814163c99213d7a8ee2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:develop` - linux; amd64

```console
$ docker pull eggdrop@sha256:4212753377a2c6e4c068a70d5449af9847392ea13aa56445ece664211f6f67aa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13902137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17330993d052321143dca954dfef6d157773551ae861dfd210bdcf7cfb674497`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:19 GMT
ADD file:c744c1dc3da4145771e66d90e2e97a4f7fb702e5e07cf4e766ee0792cf161d92 in / 
# Wed, 31 Mar 2021 20:10:19 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 14:09:11 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 01 Apr 2021 14:09:12 GMT
RUN adduser -S eggdrop
# Thu, 01 Apr 2021 14:09:13 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 01 Apr 2021 14:09:14 GMT
ENV EGGDROP_SHA256=ef482116819630aa65127d1c3d04e3762cbf45827bc66d7d505d481960209448
# Thu, 01 Apr 2021 14:09:14 GMT
ENV EGGDROP_COMMIT=d7729c4bbfb30e831e879da3985832e1db503dff
# Thu, 01 Apr 2021 14:09:15 GMT
RUN apk --update add --no-cache tcl bash openssl
# Thu, 01 Apr 2021 14:10:06 GMT
RUN apk --update add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256  develop.tar.gz" | sha256sum -c -   && tar -zxvf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 01 Apr 2021 14:10:07 GMT
ENV NICK=
# Thu, 01 Apr 2021 14:10:07 GMT
ENV SERVER=
# Thu, 01 Apr 2021 14:10:07 GMT
ENV LISTEN=3333
# Thu, 01 Apr 2021 14:10:07 GMT
ENV OWNER=
# Thu, 01 Apr 2021 14:10:07 GMT
ENV USERFILE=eggdrop.user
# Thu, 01 Apr 2021 14:10:08 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 01 Apr 2021 14:10:08 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 01 Apr 2021 14:10:08 GMT
EXPOSE 3333
# Thu, 01 Apr 2021 14:10:08 GMT
COPY file:4b2e5310f8e2b48c1ffa7bba797207637a35204a73634e98dc622889d320f394 in /home/eggdrop/eggdrop 
# Thu, 01 Apr 2021 14:10:08 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 01 Apr 2021 14:10:09 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 01 Apr 2021 14:10:09 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:9b794450f7b6db7c944ba1f4161edb68cb535052fe7db8ac06e613516c4a658d`  
		Last Modified: Wed, 31 Mar 2021 20:11:14 GMT  
		Size: 2.8 MB (2815346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed84f7efd166b1070b42b6994e6da33ee637793913d48fe14d6d8bbdc47c117e`  
		Last Modified: Thu, 01 Apr 2021 14:12:52 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a29b133e46ca39bfc1b53c0577ba915d723b6f9817b1f7f5923bf15c42a6b07`  
		Last Modified: Thu, 01 Apr 2021 14:12:47 GMT  
		Size: 9.6 KB (9585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e31fecc5bb774de853aa4cdfa1d32335dc5a5dd855e87d645044f3caca5bd0a`  
		Last Modified: Thu, 01 Apr 2021 14:12:49 GMT  
		Size: 2.7 MB (2685252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec24b445a2759e99700c2cf014cfac28d832eceedc85fc158c1cb0387bf4d98`  
		Last Modified: Thu, 01 Apr 2021 14:12:51 GMT  
		Size: 8.4 MB (8388115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aab1a96960fceaf737f70ac9782da9b7334daf50afa768484cd80c62a8a34b0`  
		Last Modified: Thu, 01 Apr 2021 14:12:47 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b191533e1841e4dc2ea57ebe4589e66331c3c2f9634429517f9db466c07e45b9`  
		Last Modified: Thu, 01 Apr 2021 14:12:47 GMT  
		Size: 697.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:1ce68c61ea440dd7733279b13f6702c3d125a79dc726c20413e832260d105324
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13559845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3796390274648c0cd10658c423df02cbf1846f19880af1cfb795210698ff7f01`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:20 GMT
ADD file:15a1f9d3700deb648f0b3701afebc97ff28eb30d1b55e18dc9c696a9dd5c8e36 in / 
# Wed, 31 Mar 2021 17:19:21 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 19:26:14 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Wed, 31 Mar 2021 19:26:17 GMT
RUN adduser -S eggdrop
# Wed, 31 Mar 2021 19:26:20 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 31 Mar 2021 19:26:21 GMT
ENV EGGDROP_SHA256=ef482116819630aa65127d1c3d04e3762cbf45827bc66d7d505d481960209448
# Wed, 31 Mar 2021 19:26:22 GMT
ENV EGGDROP_COMMIT=d7729c4bbfb30e831e879da3985832e1db503dff
# Wed, 31 Mar 2021 19:26:26 GMT
RUN apk --update add --no-cache tcl bash openssl
# Wed, 31 Mar 2021 19:28:30 GMT
RUN apk --update add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256  develop.tar.gz" | sha256sum -c -   && tar -zxvf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Wed, 31 Mar 2021 19:28:32 GMT
ENV NICK=
# Wed, 31 Mar 2021 19:28:34 GMT
ENV SERVER=
# Wed, 31 Mar 2021 19:28:35 GMT
ENV LISTEN=3333
# Wed, 31 Mar 2021 19:28:37 GMT
ENV OWNER=
# Wed, 31 Mar 2021 19:28:38 GMT
ENV USERFILE=eggdrop.user
# Wed, 31 Mar 2021 19:28:40 GMT
ENV CHANFILE=eggdrop.chan
# Wed, 31 Mar 2021 19:28:42 GMT
WORKDIR /home/eggdrop/eggdrop
# Wed, 31 Mar 2021 19:28:43 GMT
EXPOSE 3333
# Wed, 31 Mar 2021 19:28:44 GMT
COPY file:4b2e5310f8e2b48c1ffa7bba797207637a35204a73634e98dc622889d320f394 in /home/eggdrop/eggdrop 
# Wed, 31 Mar 2021 19:28:45 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Wed, 31 Mar 2021 19:28:47 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Wed, 31 Mar 2021 19:28:48 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:ac95243af174972febc49043f62f7b952a0c610e59b55ac4133f442e399e8729`  
		Last Modified: Wed, 31 Mar 2021 17:20:17 GMT  
		Size: 2.6 MB (2621248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ecba002b2ff0ad904738eaa865c25b258e83db29922d90e3dc6e1c0c9e15026`  
		Last Modified: Wed, 31 Mar 2021 19:32:52 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc7644397cfc7756dd7f29c945dbf615e503c9633839b1484ae84d6332ad3458`  
		Last Modified: Wed, 31 Mar 2021 19:32:50 GMT  
		Size: 9.4 KB (9401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfaafce071e2fc9a9b8d54defb4dab1b760de96e566c70cf167b43de05e2975a`  
		Last Modified: Wed, 31 Mar 2021 19:32:51 GMT  
		Size: 2.6 MB (2608721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6306f658ecba7e7acb7298eca26a602ece57f803e2cbae60edf3760b037b1c63`  
		Last Modified: Wed, 31 Mar 2021 19:32:55 GMT  
		Size: 8.3 MB (8316631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ef6d5a928f32740a1735dc5ef697c83e9d572fa7f9b48e7723ba979f6fc5c6`  
		Last Modified: Wed, 31 Mar 2021 19:32:52 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aedfadecf8d60c8b60d94b6651a8b0cfbdd24047175175c72ede78ebe2648450`  
		Last Modified: Wed, 31 Mar 2021 19:32:50 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:39782ca2e2f027dcaee1134f229d5d1e40964b7ea28cc1acdd55297c83b429e4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13868582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:833b296620c2c8f412b2bbf86bf4a94d8cb9876112ff6ec4a324d0225a54d026`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:22:02 GMT
ADD file:174ba1b913c5cf549fcdfc259e8e3aa8f49cea660865fd54b8aacb430602a783 in / 
# Wed, 31 Mar 2021 17:22:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:28:17 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Thu, 01 Apr 2021 13:28:20 GMT
RUN adduser -S eggdrop
# Thu, 01 Apr 2021 13:28:24 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 01 Apr 2021 13:28:25 GMT
ENV EGGDROP_SHA256=ef482116819630aa65127d1c3d04e3762cbf45827bc66d7d505d481960209448
# Thu, 01 Apr 2021 13:28:26 GMT
ENV EGGDROP_COMMIT=d7729c4bbfb30e831e879da3985832e1db503dff
# Thu, 01 Apr 2021 13:28:29 GMT
RUN apk --update add --no-cache tcl bash openssl
# Thu, 01 Apr 2021 13:30:26 GMT
RUN apk --update add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256  develop.tar.gz" | sha256sum -c -   && tar -zxvf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 01 Apr 2021 13:30:29 GMT
ENV NICK=
# Thu, 01 Apr 2021 13:30:31 GMT
ENV SERVER=
# Thu, 01 Apr 2021 13:30:32 GMT
ENV LISTEN=3333
# Thu, 01 Apr 2021 13:30:34 GMT
ENV OWNER=
# Thu, 01 Apr 2021 13:30:36 GMT
ENV USERFILE=eggdrop.user
# Thu, 01 Apr 2021 13:30:37 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 01 Apr 2021 13:30:38 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 01 Apr 2021 13:30:39 GMT
EXPOSE 3333
# Thu, 01 Apr 2021 13:30:40 GMT
COPY file:4b2e5310f8e2b48c1ffa7bba797207637a35204a73634e98dc622889d320f394 in /home/eggdrop/eggdrop 
# Thu, 01 Apr 2021 13:30:41 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 01 Apr 2021 13:30:42 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 01 Apr 2021 13:30:43 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:a3cf95b55367cb73f51318ee9c854def347373482336709ca1882a5d4c20b7c7`  
		Last Modified: Wed, 31 Mar 2021 17:23:00 GMT  
		Size: 2.7 MB (2725871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:188afabcb63d0738806b1833a44dd902f7084e613bcbe2c56cc8d0d387f15632`  
		Last Modified: Thu, 01 Apr 2021 13:33:35 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3a618ab53e63f25d0bd2b96855f67e6329c2e62fb4106104979292ba8e3522`  
		Last Modified: Thu, 01 Apr 2021 13:33:34 GMT  
		Size: 9.5 KB (9515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f65969fa81374b8aaba7467f1c9c4e4dd6a458362dcf46467fc48def596f8d8`  
		Last Modified: Thu, 01 Apr 2021 13:33:35 GMT  
		Size: 2.7 MB (2722554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293fca9a44b4f3fc7bac8b9859c8618ebc45e0a025891ce5c930c0bee4c1889f`  
		Last Modified: Thu, 01 Apr 2021 13:33:36 GMT  
		Size: 8.4 MB (8406789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4cae91dfdf7a3196b735816f6eb0bbd8079d1e0bb07dadce8a0c47a56f2e20`  
		Last Modified: Thu, 01 Apr 2021 13:33:34 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e43dca60489d3d5bd9b761d05f89836df5b77ec2310c2b7f7ba32f0717dfb9a`  
		Last Modified: Thu, 01 Apr 2021 13:33:34 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
