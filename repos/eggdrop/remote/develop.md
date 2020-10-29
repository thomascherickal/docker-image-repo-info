## `eggdrop:develop`

```console
$ docker pull eggdrop@sha256:8ab44777d2aa0c412d05a58290d26f50a2b273a3651bdde0205f1910945a4d0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `eggdrop:develop` - linux; amd64

```console
$ docker pull eggdrop@sha256:075ac1b940cd44864b8ca5408cf08d75907b293b5a80ad5f64cf5bc398fd1c38
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.2 MB (13229449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21d48351a13e51ee145c77cf30f9b65bd4ddfc3eb1fda136c8051815df17df61`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:21:14 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Fri, 24 Apr 2020 14:21:15 GMT
RUN adduser -S eggdrop
# Fri, 24 Apr 2020 14:21:16 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 29 Oct 2020 18:19:35 GMT
ENV EGGDROP_SHA256=c03b55ff977b671d5d43bfc2956294ec31bda1936ec0520b260c7e7020c6f656
# Thu, 29 Oct 2020 18:19:35 GMT
ENV EGGDROP_COMMIT=a2bd85e40c85a6dcfaf8d0f11bb7967f82ac67a1
# Thu, 29 Oct 2020 18:19:36 GMT
RUN apk --update add --no-cache tcl bash openssl
# Thu, 29 Oct 2020 18:20:33 GMT
RUN apk --update add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256  develop.tar.gz" | sha256sum -c -   && tar -zxvf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 29 Oct 2020 18:20:33 GMT
ENV NICK=
# Thu, 29 Oct 2020 18:20:33 GMT
ENV SERVER=
# Thu, 29 Oct 2020 18:20:34 GMT
ENV LISTEN=3333
# Thu, 29 Oct 2020 18:20:34 GMT
ENV OWNER=
# Thu, 29 Oct 2020 18:20:34 GMT
ENV USERFILE=eggdrop.user
# Thu, 29 Oct 2020 18:20:34 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 29 Oct 2020 18:20:34 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 29 Oct 2020 18:20:35 GMT
EXPOSE 3333
# Thu, 29 Oct 2020 18:20:35 GMT
COPY file:4b2e5310f8e2b48c1ffa7bba797207637a35204a73634e98dc622889d320f394 in /home/eggdrop/eggdrop 
# Thu, 29 Oct 2020 18:20:35 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 29 Oct 2020 18:20:35 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 29 Oct 2020 18:20:35 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0cdf0ff845235e19454000f632a4d9bf6d978c7948da54b51bf3962d766f4c`  
		Last Modified: Fri, 24 Apr 2020 14:23:40 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05e553ff44d8d1344fff59fed8897d80984977807b655be3d15128815d5bcf0`  
		Last Modified: Fri, 24 Apr 2020 14:23:38 GMT  
		Size: 9.6 KB (9573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a949cc28cd9cf9019880fd8c36705e696b7d085bb54a9deeae8c234e35299af0`  
		Last Modified: Thu, 29 Oct 2020 18:20:48 GMT  
		Size: 2.7 MB (2685008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818a418e65bd8fdd52d06302d489bdf88c0cb7332839c5e8204de9b5f20a4205`  
		Last Modified: Thu, 29 Oct 2020 18:20:49 GMT  
		Size: 7.7 MB (7717723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c154fb957a3cf4f88473f05e485108ae9423bd3b3b758fddac43879beb978af`  
		Last Modified: Thu, 29 Oct 2020 18:20:48 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf84d87b4a63bc74493f01f6ed30547171e39b866fca484e05af2228a766a9f2`  
		Last Modified: Thu, 29 Oct 2020 18:20:48 GMT  
		Size: 707.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm variant v6

```console
$ docker pull eggdrop@sha256:e25554b97cdc6cdc360ce15440d06b669bb96de35066c3feb02c7228d616f0a6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.9 MB (12897664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5c405c23e3b17c5806747d2193838cc1b1a2692e67cbbccaa134aeb87f54b24`
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
# Thu, 29 Oct 2020 18:51:03 GMT
ENV EGGDROP_SHA256=c03b55ff977b671d5d43bfc2956294ec31bda1936ec0520b260c7e7020c6f656
# Thu, 29 Oct 2020 18:51:03 GMT
ENV EGGDROP_COMMIT=a2bd85e40c85a6dcfaf8d0f11bb7967f82ac67a1
# Thu, 29 Oct 2020 18:51:07 GMT
RUN apk --update add --no-cache tcl bash openssl
# Thu, 29 Oct 2020 18:52:57 GMT
RUN apk --update add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256  develop.tar.gz" | sha256sum -c -   && tar -zxvf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 29 Oct 2020 18:52:57 GMT
ENV NICK=
# Thu, 29 Oct 2020 18:52:58 GMT
ENV SERVER=
# Thu, 29 Oct 2020 18:52:59 GMT
ENV LISTEN=3333
# Thu, 29 Oct 2020 18:53:00 GMT
ENV OWNER=
# Thu, 29 Oct 2020 18:53:01 GMT
ENV USERFILE=eggdrop.user
# Thu, 29 Oct 2020 18:53:02 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 29 Oct 2020 18:53:03 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 29 Oct 2020 18:53:04 GMT
EXPOSE 3333
# Thu, 29 Oct 2020 18:53:05 GMT
COPY file:4b2e5310f8e2b48c1ffa7bba797207637a35204a73634e98dc622889d320f394 in /home/eggdrop/eggdrop 
# Thu, 29 Oct 2020 18:53:05 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 29 Oct 2020 18:53:06 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 29 Oct 2020 18:53:07 GMT
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
	-	`sha256:d7edcf0bf6e273b45744d67c42d5fcc87f1ea5ba3c9ad507a682f01e5a160052`  
		Last Modified: Thu, 29 Oct 2020 18:53:25 GMT  
		Size: 2.6 MB (2608672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10b52e0422e4f01462fe1c6a05308da375b089d3dea978b996b53aa460e1d55`  
		Last Modified: Thu, 29 Oct 2020 18:53:26 GMT  
		Size: 7.7 MB (7655809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc734fb4d106f4809e78cacfee43b4ef684bd5836dd2a8a540ff0972a54b72f`  
		Last Modified: Thu, 29 Oct 2020 18:53:23 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:106651e0137d857844d51de4be8294d8278ba629c51cbe90af410aaf4c30512e`  
		Last Modified: Thu, 29 Oct 2020 18:53:24 GMT  
		Size: 709.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eggdrop:develop` - linux; arm64 variant v8

```console
$ docker pull eggdrop@sha256:8b92a1177e2caa4633fe60b363f6f4f834013da7c33fd3a1c56d4c5887ff4d01
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.2 MB (13193257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20fd28abeb935cb177b40b662a24f6d68880943154c1a8e772c34650b7a2f3a3`
-	Entrypoint: `["\/home\/eggdrop\/eggdrop\/entrypoint.sh"]`
-	Default Command: `["eggdrop.conf"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:02:28 GMT
MAINTAINER Geo Van O <geo@eggheads.org>
# Fri, 24 Apr 2020 09:02:31 GMT
RUN adduser -S eggdrop
# Fri, 24 Apr 2020 09:02:34 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 29 Oct 2020 18:39:49 GMT
ENV EGGDROP_SHA256=c03b55ff977b671d5d43bfc2956294ec31bda1936ec0520b260c7e7020c6f656
# Thu, 29 Oct 2020 18:39:50 GMT
ENV EGGDROP_COMMIT=a2bd85e40c85a6dcfaf8d0f11bb7967f82ac67a1
# Thu, 29 Oct 2020 18:39:53 GMT
RUN apk --update add --no-cache tcl bash openssl
# Thu, 29 Oct 2020 18:41:35 GMT
RUN apk --update add --no-cache --virtual egg-deps tcl-dev wget ca-certificates make tar gpgme build-base openssl-dev   && wget "https://github.com/eggheads/eggdrop/archive/$EGGDROP_COMMIT.tar.gz" -O develop.tar.gz   && echo "$EGGDROP_SHA256  develop.tar.gz" | sha256sum -c -   && tar -zxvf develop.tar.gz   && rm develop.tar.gz     && ( cd eggdrop-$EGGDROP_COMMIT     && ./configure     && make config     && make     && make install DEST=/home/eggdrop/eggdrop )   && rm -rf eggdrop-$EGGDROP_COMMIT   && mkdir /home/eggdrop/eggdrop/data   && chown -R eggdrop /home/eggdrop/eggdrop   && apk del egg-deps
# Thu, 29 Oct 2020 18:41:36 GMT
ENV NICK=
# Thu, 29 Oct 2020 18:41:36 GMT
ENV SERVER=
# Thu, 29 Oct 2020 18:41:37 GMT
ENV LISTEN=3333
# Thu, 29 Oct 2020 18:41:37 GMT
ENV OWNER=
# Thu, 29 Oct 2020 18:41:38 GMT
ENV USERFILE=eggdrop.user
# Thu, 29 Oct 2020 18:41:38 GMT
ENV CHANFILE=eggdrop.chan
# Thu, 29 Oct 2020 18:41:39 GMT
WORKDIR /home/eggdrop/eggdrop
# Thu, 29 Oct 2020 18:41:39 GMT
EXPOSE 3333
# Thu, 29 Oct 2020 18:41:40 GMT
COPY file:4b2e5310f8e2b48c1ffa7bba797207637a35204a73634e98dc622889d320f394 in /home/eggdrop/eggdrop 
# Thu, 29 Oct 2020 18:41:41 GMT
COPY file:b76e92fb28997fa3fd71a3b880ff3b73567ca05021b617d51ebdcefd8c31b457 in /home/eggdrop/eggdrop/scripts/ 
# Thu, 29 Oct 2020 18:41:41 GMT
ENTRYPOINT ["/home/eggdrop/eggdrop/entrypoint.sh"]
# Thu, 29 Oct 2020 18:41:42 GMT
CMD ["eggdrop.conf"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:848a8db5818fe5b735a8e3706dd1ae7043eb3b468306058c8c416fb4770df991`  
		Last Modified: Fri, 24 Apr 2020 09:04:52 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdba78ca0222af81b132121091d817259b1a4e7a7e98379b4dcaec6e64d10a2c`  
		Last Modified: Fri, 24 Apr 2020 09:04:50 GMT  
		Size: 9.5 KB (9514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ab0862a4232552601797bb7d0c477c6b2de4cfd5e9e90064549e37dcf57727`  
		Last Modified: Thu, 29 Oct 2020 18:41:57 GMT  
		Size: 2.7 MB (2722570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9bc8709503e84c22883634cd897d04153c4d71d46692ef0f8f7a606f79d7511`  
		Last Modified: Thu, 29 Oct 2020 18:41:59 GMT  
		Size: 7.7 MB (7732889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b3803bbcecd6a688a009cc7827a6a373fd388720225aaf8fe98aa47fa2321f`  
		Last Modified: Thu, 29 Oct 2020 18:41:57 GMT  
		Size: 1.9 KB (1887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4253e1db1b3fe2a97b451102e51726e9bf4fd57be04e0aea6322656b9b6abae3`  
		Last Modified: Thu, 29 Oct 2020 18:41:56 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
