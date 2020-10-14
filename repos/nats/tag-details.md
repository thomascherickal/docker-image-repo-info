<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats`

-	[`nats:2`](#nats2)
-	[`nats:2.1`](#nats21)
-	[`nats:2.1.8`](#nats218)
-	[`nats:2.1.8-alpine`](#nats218-alpine)
-	[`nats:2.1.8-alpine3.11`](#nats218-alpine311)
-	[`nats:2.1.8-linux`](#nats218-linux)
-	[`nats:2.1.8-nanoserver`](#nats218-nanoserver)
-	[`nats:2.1.8-nanoserver-1809`](#nats218-nanoserver-1809)
-	[`nats:2.1.8-scratch`](#nats218-scratch)
-	[`nats:2.1.8-windowsservercore`](#nats218-windowsservercore)
-	[`nats:2.1.8-windowsservercore-1809`](#nats218-windowsservercore-1809)
-	[`nats:2.1.8-windowsservercore-ltsc2016`](#nats218-windowsservercore-ltsc2016)
-	[`nats:2.1-alpine`](#nats21-alpine)
-	[`nats:2.1-alpine3.11`](#nats21-alpine311)
-	[`nats:2.1-linux`](#nats21-linux)
-	[`nats:2.1-nanoserver`](#nats21-nanoserver)
-	[`nats:2.1-nanoserver-1809`](#nats21-nanoserver-1809)
-	[`nats:2.1-scratch`](#nats21-scratch)
-	[`nats:2.1-windowsservercore`](#nats21-windowsservercore)
-	[`nats:2.1-windowsservercore-1809`](#nats21-windowsservercore-1809)
-	[`nats:2.1-windowsservercore-ltsc2016`](#nats21-windowsservercore-ltsc2016)
-	[`nats:2-alpine`](#nats2-alpine)
-	[`nats:2-alpine3.11`](#nats2-alpine311)
-	[`nats:2-linux`](#nats2-linux)
-	[`nats:2-nanoserver`](#nats2-nanoserver)
-	[`nats:2-nanoserver-1809`](#nats2-nanoserver-1809)
-	[`nats:2-scratch`](#nats2-scratch)
-	[`nats:2-windowsservercore`](#nats2-windowsservercore)
-	[`nats:2-windowsservercore-1809`](#nats2-windowsservercore-1809)
-	[`nats:2-windowsservercore-ltsc2016`](#nats2-windowsservercore-ltsc2016)
-	[`nats:alpine`](#natsalpine)
-	[`nats:alpine3.11`](#natsalpine311)
-	[`nats:latest`](#natslatest)
-	[`nats:linux`](#natslinux)
-	[`nats:nanoserver`](#natsnanoserver)
-	[`nats:nanoserver-1809`](#natsnanoserver-1809)
-	[`nats:scratch`](#natsscratch)
-	[`nats:windowsservercore`](#natswindowsservercore)
-	[`nats:windowsservercore-1809`](#natswindowsservercore-1809)
-	[`nats:windowsservercore-ltsc2016`](#natswindowsservercore-ltsc2016)

## `nats:2`

```console
$ docker pull nats@sha256:d24378f3491a4ba21c6ec5cddd787f7d4b8004d045ff9fe227037d12491f375e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1518; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:0d7c496dd4f8512bf5c61832bc16e75d805de038fc08554f33fefbcd3907c4b2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4093542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8a33d0935d56b4724ba17d1c68ebc2c6abeab51f35b5c0a9d44bb9749d251c6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 19:24:31 GMT
COPY file:22772fe85f23ca6ef547526020b6f0c57f7bb05cf1b63d4adebc9bac5872d5ce in /nats-server 
# Fri, 04 Sep 2020 19:24:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 19:24:31 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:24:31 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 19:24:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ae9aef3549a0277b3c71f27b28f1616f87abeb4dfcec5ff0f2bb2109fb259b34`  
		Last Modified: Fri, 04 Sep 2020 19:25:04 GMT  
		Size: 4.1 MB (4093066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee674f246b57d546774a96e8caa7a1528c4400b153e22ce806dc1c2cb079a2e9`  
		Last Modified: Fri, 04 Sep 2020 19:25:03 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:4d7a3526a49cff86b7b08e7754e694bc8debf597effe86c2507fdd4ea32487c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3815178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e62937d0c25fb6d311b12f184e3caa42b65ff2d3988db590064304ff0419db92`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 08 Sep 2020 20:53:16 GMT
COPY file:2414e6a1d4e6c04ea1bd45da76034c284460c92fcf95b5375100eb111f6bcb4f in /nats-server 
# Tue, 08 Sep 2020 20:53:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 08 Sep 2020 20:53:32 GMT
EXPOSE 4222 6222 8222
# Tue, 08 Sep 2020 20:53:37 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 08 Sep 2020 20:53:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:22845e86cdccc8a91bee01c29a4508fa756a18313163373688eadb71457dd1ab`  
		Last Modified: Tue, 08 Sep 2020 20:55:13 GMT  
		Size: 3.8 MB (3814699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048bf9997f96f5831b0b020d70687709d3e7edc8b3cc13fb11363f7bafd6e319`  
		Last Modified: Tue, 08 Sep 2020 20:55:11 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:20ea87b418a2b1273123ddef4c91956990c5fcab0bbad71523d5b6b434be249c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3811018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0459d9344473c88c51591d37f17b57327d167b6122217d7422431b328c3a1b02`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 20:10:08 GMT
COPY file:3ebd94b1867641b7e927368abdd7734a27a700b6431d3d384660c98fb6f91ae9 in /nats-server 
# Fri, 04 Sep 2020 20:10:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 20:10:26 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 20:10:31 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 20:10:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9388f799ec4c0c97ac0c4f5d9d8936ef881f647ba80558b3f746eea63397a54e`  
		Last Modified: Fri, 04 Sep 2020 20:11:29 GMT  
		Size: 3.8 MB (3810540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce31c20db639568dc0ccc4e73f1bdc208376b2a5b1633adc0587d4ff8aaf0c4`  
		Last Modified: Fri, 04 Sep 2020 20:11:27 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:46cae43c1deb7bbc919efb2f3271f78e195f1eaa3f8b626376dfdb633ff3b555
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3792562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71a111e279efaf7a4228a57b652684e1adf34e569fc9e077ecd7350dcb0aac50`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 19:51:03 GMT
COPY file:c0962878fe6b8c789e4fa27fcefd32cc868d740092dee272d993d0aac72edeca in /nats-server 
# Fri, 04 Sep 2020 19:51:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 19:51:04 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:51:05 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 19:51:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:176dd0e74c68ca9b537d3cde057424bc8bf3cff7d363d760f1ad421beaef143f`  
		Last Modified: Fri, 04 Sep 2020 19:51:45 GMT  
		Size: 3.8 MB (3792086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b07612acf847f5e6dc42a05a50dbe09be5e7de55f6028a850048895ff39137`  
		Last Modified: Fri, 04 Sep 2020 19:51:44 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.1518; amd64

```console
$ docker pull nats@sha256:2bb0cf3737e6f9280c017d9f69a0dd3cc87cd19970c590c82c9bc8a21b465caa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105248098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:784ca74fae547093d5ec6324890b5524d17bab6ec9f6081dd1e10a2b1ebad657`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 30 Sep 2020 11:25:56 GMT
RUN Apply image 1809-amd64
# Wed, 14 Oct 2020 16:26:27 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 16:26:28 GMT
RUN cmd /S /C #(nop) COPY file:0b6475b59bf6bfe6c1030fd41ea501af74fd46ae70fd98c58683b35f8ed498ff in C:\nats-server.exe 
# Wed, 14 Oct 2020 16:26:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Oct 2020 16:26:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Oct 2020 16:26:31 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Oct 2020 16:26:32 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aab6118ce69c93410df7fa15842a6e3b3c7ff20b639c779b5d5f78e7653eaa07`  
		Size: 101.2 MB (101205155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:93b9a3c3e46fc1677426e3be7ce449b91d540c5ae2147380034cc4e1dc7445c3`  
		Last Modified: Wed, 14 Oct 2020 16:31:12 GMT  
		Size: 910.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f192833ce36b0638e48f194ecb14073cd09261d874eb20729671b313f29b3a`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 4.0 MB (4037949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adf949cd79179965570b7d54d6e187eab3a6a5fda1ae9bc15c56233fc001be9`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 1.5 KB (1496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bc641bd835d0a958bbb4a03d9629ffab985d2bde1b52bfeacf45583a784e40`  
		Last Modified: Wed, 14 Oct 2020 16:31:09 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9f9dddc4fec5b66e7c7189d7aa273a6021bfb1c2268ac7cdde04effab31105`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391656292799f8f1ed48dd6d84a3b168cadd87a302f37822617602b6edfa2bbc`  
		Last Modified: Wed, 14 Oct 2020 16:31:14 GMT  
		Size: 865.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1`

```console
$ docker pull nats@sha256:d24378f3491a4ba21c6ec5cddd787f7d4b8004d045ff9fe227037d12491f375e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1518; amd64

### `nats:2.1` - linux; amd64

```console
$ docker pull nats@sha256:0d7c496dd4f8512bf5c61832bc16e75d805de038fc08554f33fefbcd3907c4b2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4093542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8a33d0935d56b4724ba17d1c68ebc2c6abeab51f35b5c0a9d44bb9749d251c6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 19:24:31 GMT
COPY file:22772fe85f23ca6ef547526020b6f0c57f7bb05cf1b63d4adebc9bac5872d5ce in /nats-server 
# Fri, 04 Sep 2020 19:24:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 19:24:31 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:24:31 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 19:24:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ae9aef3549a0277b3c71f27b28f1616f87abeb4dfcec5ff0f2bb2109fb259b34`  
		Last Modified: Fri, 04 Sep 2020 19:25:04 GMT  
		Size: 4.1 MB (4093066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee674f246b57d546774a96e8caa7a1528c4400b153e22ce806dc1c2cb079a2e9`  
		Last Modified: Fri, 04 Sep 2020 19:25:03 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1` - linux; arm variant v6

```console
$ docker pull nats@sha256:4d7a3526a49cff86b7b08e7754e694bc8debf597effe86c2507fdd4ea32487c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3815178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e62937d0c25fb6d311b12f184e3caa42b65ff2d3988db590064304ff0419db92`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 08 Sep 2020 20:53:16 GMT
COPY file:2414e6a1d4e6c04ea1bd45da76034c284460c92fcf95b5375100eb111f6bcb4f in /nats-server 
# Tue, 08 Sep 2020 20:53:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 08 Sep 2020 20:53:32 GMT
EXPOSE 4222 6222 8222
# Tue, 08 Sep 2020 20:53:37 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 08 Sep 2020 20:53:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:22845e86cdccc8a91bee01c29a4508fa756a18313163373688eadb71457dd1ab`  
		Last Modified: Tue, 08 Sep 2020 20:55:13 GMT  
		Size: 3.8 MB (3814699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048bf9997f96f5831b0b020d70687709d3e7edc8b3cc13fb11363f7bafd6e319`  
		Last Modified: Tue, 08 Sep 2020 20:55:11 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1` - linux; arm variant v7

```console
$ docker pull nats@sha256:20ea87b418a2b1273123ddef4c91956990c5fcab0bbad71523d5b6b434be249c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3811018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0459d9344473c88c51591d37f17b57327d167b6122217d7422431b328c3a1b02`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 20:10:08 GMT
COPY file:3ebd94b1867641b7e927368abdd7734a27a700b6431d3d384660c98fb6f91ae9 in /nats-server 
# Fri, 04 Sep 2020 20:10:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 20:10:26 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 20:10:31 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 20:10:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9388f799ec4c0c97ac0c4f5d9d8936ef881f647ba80558b3f746eea63397a54e`  
		Last Modified: Fri, 04 Sep 2020 20:11:29 GMT  
		Size: 3.8 MB (3810540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce31c20db639568dc0ccc4e73f1bdc208376b2a5b1633adc0587d4ff8aaf0c4`  
		Last Modified: Fri, 04 Sep 2020 20:11:27 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:46cae43c1deb7bbc919efb2f3271f78e195f1eaa3f8b626376dfdb633ff3b555
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3792562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71a111e279efaf7a4228a57b652684e1adf34e569fc9e077ecd7350dcb0aac50`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 19:51:03 GMT
COPY file:c0962878fe6b8c789e4fa27fcefd32cc868d740092dee272d993d0aac72edeca in /nats-server 
# Fri, 04 Sep 2020 19:51:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 19:51:04 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:51:05 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 19:51:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:176dd0e74c68ca9b537d3cde057424bc8bf3cff7d363d760f1ad421beaef143f`  
		Last Modified: Fri, 04 Sep 2020 19:51:45 GMT  
		Size: 3.8 MB (3792086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b07612acf847f5e6dc42a05a50dbe09be5e7de55f6028a850048895ff39137`  
		Last Modified: Fri, 04 Sep 2020 19:51:44 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1` - windows version 10.0.17763.1518; amd64

```console
$ docker pull nats@sha256:2bb0cf3737e6f9280c017d9f69a0dd3cc87cd19970c590c82c9bc8a21b465caa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105248098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:784ca74fae547093d5ec6324890b5524d17bab6ec9f6081dd1e10a2b1ebad657`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 30 Sep 2020 11:25:56 GMT
RUN Apply image 1809-amd64
# Wed, 14 Oct 2020 16:26:27 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 16:26:28 GMT
RUN cmd /S /C #(nop) COPY file:0b6475b59bf6bfe6c1030fd41ea501af74fd46ae70fd98c58683b35f8ed498ff in C:\nats-server.exe 
# Wed, 14 Oct 2020 16:26:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Oct 2020 16:26:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Oct 2020 16:26:31 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Oct 2020 16:26:32 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aab6118ce69c93410df7fa15842a6e3b3c7ff20b639c779b5d5f78e7653eaa07`  
		Size: 101.2 MB (101205155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:93b9a3c3e46fc1677426e3be7ce449b91d540c5ae2147380034cc4e1dc7445c3`  
		Last Modified: Wed, 14 Oct 2020 16:31:12 GMT  
		Size: 910.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f192833ce36b0638e48f194ecb14073cd09261d874eb20729671b313f29b3a`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 4.0 MB (4037949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adf949cd79179965570b7d54d6e187eab3a6a5fda1ae9bc15c56233fc001be9`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 1.5 KB (1496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bc641bd835d0a958bbb4a03d9629ffab985d2bde1b52bfeacf45583a784e40`  
		Last Modified: Wed, 14 Oct 2020 16:31:09 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9f9dddc4fec5b66e7c7189d7aa273a6021bfb1c2268ac7cdde04effab31105`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391656292799f8f1ed48dd6d84a3b168cadd87a302f37822617602b6edfa2bbc`  
		Last Modified: Wed, 14 Oct 2020 16:31:14 GMT  
		Size: 865.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.8`

```console
$ docker pull nats@sha256:d24378f3491a4ba21c6ec5cddd787f7d4b8004d045ff9fe227037d12491f375e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1518; amd64

### `nats:2.1.8` - linux; amd64

```console
$ docker pull nats@sha256:0d7c496dd4f8512bf5c61832bc16e75d805de038fc08554f33fefbcd3907c4b2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4093542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8a33d0935d56b4724ba17d1c68ebc2c6abeab51f35b5c0a9d44bb9749d251c6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 19:24:31 GMT
COPY file:22772fe85f23ca6ef547526020b6f0c57f7bb05cf1b63d4adebc9bac5872d5ce in /nats-server 
# Fri, 04 Sep 2020 19:24:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 19:24:31 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:24:31 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 19:24:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ae9aef3549a0277b3c71f27b28f1616f87abeb4dfcec5ff0f2bb2109fb259b34`  
		Last Modified: Fri, 04 Sep 2020 19:25:04 GMT  
		Size: 4.1 MB (4093066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee674f246b57d546774a96e8caa7a1528c4400b153e22ce806dc1c2cb079a2e9`  
		Last Modified: Fri, 04 Sep 2020 19:25:03 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.8` - linux; arm variant v6

```console
$ docker pull nats@sha256:4d7a3526a49cff86b7b08e7754e694bc8debf597effe86c2507fdd4ea32487c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3815178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e62937d0c25fb6d311b12f184e3caa42b65ff2d3988db590064304ff0419db92`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 08 Sep 2020 20:53:16 GMT
COPY file:2414e6a1d4e6c04ea1bd45da76034c284460c92fcf95b5375100eb111f6bcb4f in /nats-server 
# Tue, 08 Sep 2020 20:53:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 08 Sep 2020 20:53:32 GMT
EXPOSE 4222 6222 8222
# Tue, 08 Sep 2020 20:53:37 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 08 Sep 2020 20:53:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:22845e86cdccc8a91bee01c29a4508fa756a18313163373688eadb71457dd1ab`  
		Last Modified: Tue, 08 Sep 2020 20:55:13 GMT  
		Size: 3.8 MB (3814699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048bf9997f96f5831b0b020d70687709d3e7edc8b3cc13fb11363f7bafd6e319`  
		Last Modified: Tue, 08 Sep 2020 20:55:11 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.8` - linux; arm variant v7

```console
$ docker pull nats@sha256:20ea87b418a2b1273123ddef4c91956990c5fcab0bbad71523d5b6b434be249c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3811018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0459d9344473c88c51591d37f17b57327d167b6122217d7422431b328c3a1b02`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 20:10:08 GMT
COPY file:3ebd94b1867641b7e927368abdd7734a27a700b6431d3d384660c98fb6f91ae9 in /nats-server 
# Fri, 04 Sep 2020 20:10:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 20:10:26 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 20:10:31 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 20:10:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9388f799ec4c0c97ac0c4f5d9d8936ef881f647ba80558b3f746eea63397a54e`  
		Last Modified: Fri, 04 Sep 2020 20:11:29 GMT  
		Size: 3.8 MB (3810540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce31c20db639568dc0ccc4e73f1bdc208376b2a5b1633adc0587d4ff8aaf0c4`  
		Last Modified: Fri, 04 Sep 2020 20:11:27 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.8` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:46cae43c1deb7bbc919efb2f3271f78e195f1eaa3f8b626376dfdb633ff3b555
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3792562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71a111e279efaf7a4228a57b652684e1adf34e569fc9e077ecd7350dcb0aac50`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 19:51:03 GMT
COPY file:c0962878fe6b8c789e4fa27fcefd32cc868d740092dee272d993d0aac72edeca in /nats-server 
# Fri, 04 Sep 2020 19:51:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 19:51:04 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:51:05 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 19:51:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:176dd0e74c68ca9b537d3cde057424bc8bf3cff7d363d760f1ad421beaef143f`  
		Last Modified: Fri, 04 Sep 2020 19:51:45 GMT  
		Size: 3.8 MB (3792086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b07612acf847f5e6dc42a05a50dbe09be5e7de55f6028a850048895ff39137`  
		Last Modified: Fri, 04 Sep 2020 19:51:44 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.8` - windows version 10.0.17763.1518; amd64

```console
$ docker pull nats@sha256:2bb0cf3737e6f9280c017d9f69a0dd3cc87cd19970c590c82c9bc8a21b465caa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105248098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:784ca74fae547093d5ec6324890b5524d17bab6ec9f6081dd1e10a2b1ebad657`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 30 Sep 2020 11:25:56 GMT
RUN Apply image 1809-amd64
# Wed, 14 Oct 2020 16:26:27 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 16:26:28 GMT
RUN cmd /S /C #(nop) COPY file:0b6475b59bf6bfe6c1030fd41ea501af74fd46ae70fd98c58683b35f8ed498ff in C:\nats-server.exe 
# Wed, 14 Oct 2020 16:26:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Oct 2020 16:26:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Oct 2020 16:26:31 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Oct 2020 16:26:32 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aab6118ce69c93410df7fa15842a6e3b3c7ff20b639c779b5d5f78e7653eaa07`  
		Size: 101.2 MB (101205155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:93b9a3c3e46fc1677426e3be7ce449b91d540c5ae2147380034cc4e1dc7445c3`  
		Last Modified: Wed, 14 Oct 2020 16:31:12 GMT  
		Size: 910.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f192833ce36b0638e48f194ecb14073cd09261d874eb20729671b313f29b3a`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 4.0 MB (4037949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adf949cd79179965570b7d54d6e187eab3a6a5fda1ae9bc15c56233fc001be9`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 1.5 KB (1496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bc641bd835d0a958bbb4a03d9629ffab985d2bde1b52bfeacf45583a784e40`  
		Last Modified: Wed, 14 Oct 2020 16:31:09 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9f9dddc4fec5b66e7c7189d7aa273a6021bfb1c2268ac7cdde04effab31105`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391656292799f8f1ed48dd6d84a3b168cadd87a302f37822617602b6edfa2bbc`  
		Last Modified: Wed, 14 Oct 2020 16:31:14 GMT  
		Size: 865.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.8-alpine`

```console
$ docker pull nats@sha256:ebe6d1b23a177223608c68d8617049228b00ee54d4e758d2eca44238326b141b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.1.8-alpine` - linux; amd64

```console
$ docker pull nats@sha256:a6f914658a5f8a7a82c9005a3a36863628d331cb2cd4c0c0a3653e7e8a7c0d95
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7208222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96815e17bf1191cbfa7a1745a82f87b8fcc43fbd793da4d66c9fd175c136dd27`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 04 Sep 2020 19:23:32 GMT
ENV NATS_SERVER=2.1.8
# Fri, 04 Sep 2020 19:23:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='567d5c7f80305b8876230204b993f0cf213411d006d931a036b26dd2288ac81b' ;; 		armhf) natsArch='arm6'; sha256='d76c1ed6f660e13faaa8b1c058723981aa59436ce7d4d4e208ae486395db458f' ;; 		armv7) natsArch='arm7'; sha256='e26f0eba9b065f9537986f88233f279f44c01487aacffe65d4d7440129a5d0a2' ;; 		x86_64) natsArch='amd64'; sha256='8ec25475ef1d49bf5e721de38deb11d689d1a9b2fa588540af78d56cbea2b49d' ;; 		x86) natsArch='386'; sha256='e8535179805573e9d684cc8aa6f79551ab9fcfacd45643d7ba2174e176997d9e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 04 Sep 2020 19:23:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 04 Sep 2020 19:23:34 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Sep 2020 19:23:35 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:23:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Sep 2020 19:23:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f9fca7275bd535bd4680297f95f240c9b48d96d0b9b7f17dd38b73917d2b99`  
		Last Modified: Fri, 04 Sep 2020 19:24:56 GMT  
		Size: 4.4 MB (4393961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6905e1079d9ad73fb2f14b529adb1378cfaa4fcabf48ee0a819af4a49842a3a4`  
		Last Modified: Fri, 04 Sep 2020 19:24:55 GMT  
		Size: 530.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a148278ed7ad77a22a36b3ea6e6cdbcaa397edc556440f575992b8bbd8abfc9b`  
		Last Modified: Fri, 04 Sep 2020 19:24:55 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.8-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:66672cb8777aa5f85c15c70a90715743fcb7a4b62274bd7ce2a6eae2de23e9f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6736694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3ffd2e3668ab2027e82153bdbc9a30869007677d6a504cf12b55673d415f36f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Sep 2020 20:50:59 GMT
ENV NATS_SERVER=2.1.8
# Tue, 08 Sep 2020 20:51:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='567d5c7f80305b8876230204b993f0cf213411d006d931a036b26dd2288ac81b' ;; 		armhf) natsArch='arm6'; sha256='d76c1ed6f660e13faaa8b1c058723981aa59436ce7d4d4e208ae486395db458f' ;; 		armv7) natsArch='arm7'; sha256='e26f0eba9b065f9537986f88233f279f44c01487aacffe65d4d7440129a5d0a2' ;; 		x86_64) natsArch='amd64'; sha256='8ec25475ef1d49bf5e721de38deb11d689d1a9b2fa588540af78d56cbea2b49d' ;; 		x86) natsArch='386'; sha256='e8535179805573e9d684cc8aa6f79551ab9fcfacd45643d7ba2174e176997d9e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 08 Sep 2020 20:52:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 08 Sep 2020 20:52:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 08 Sep 2020 20:52:29 GMT
EXPOSE 4222 6222 8222
# Tue, 08 Sep 2020 20:52:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 20:52:43 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0ef3723549909739a256c2edd0d1e438f4ecd8eb6a447e818a576156017ba5`  
		Last Modified: Tue, 08 Sep 2020 20:54:21 GMT  
		Size: 4.1 MB (4115782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:495246de42a6ec596d8f30209752a4592e43515a1820cc406d2de5678b60c31b`  
		Last Modified: Tue, 08 Sep 2020 20:54:19 GMT  
		Size: 563.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28539be71de5be5dff99408931259e65df39bb85a070670d75d49f415958062`  
		Last Modified: Tue, 08 Sep 2020 20:54:18 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.8-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:645d9707a2e5fbd2330b6b7c87601978add8b5388e18c8a2dc988b2ae00bc7fd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6532999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cbe66195f5f434137dc29427ce470c725a6d3a3fb47451c0608398ec12e0749`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Fri, 04 Sep 2020 20:01:21 GMT
ENV NATS_SERVER=2.1.8
# Fri, 04 Sep 2020 20:01:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='567d5c7f80305b8876230204b993f0cf213411d006d931a036b26dd2288ac81b' ;; 		armhf) natsArch='arm6'; sha256='d76c1ed6f660e13faaa8b1c058723981aa59436ce7d4d4e208ae486395db458f' ;; 		armv7) natsArch='arm7'; sha256='e26f0eba9b065f9537986f88233f279f44c01487aacffe65d4d7440129a5d0a2' ;; 		x86_64) natsArch='amd64'; sha256='8ec25475ef1d49bf5e721de38deb11d689d1a9b2fa588540af78d56cbea2b49d' ;; 		x86) natsArch='386'; sha256='e8535179805573e9d684cc8aa6f79551ab9fcfacd45643d7ba2174e176997d9e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 04 Sep 2020 20:01:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 04 Sep 2020 20:02:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Sep 2020 20:02:18 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 20:02:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Sep 2020 20:02:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707b0a874f39e2d53e2283ffb23bd80599cd3de6fb4813b5d80b6a3576b9a285`  
		Last Modified: Fri, 04 Sep 2020 20:11:13 GMT  
		Size: 4.1 MB (4109958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66cdb37890e6affd51af4e84cb645a7bdca5322a54690e7ed1ef70fd6e7f55b9`  
		Last Modified: Fri, 04 Sep 2020 20:11:11 GMT  
		Size: 562.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358a12bb7b0cdd9809f9bcd5bf1bdbc75c5a232db47e87757596eec47fea3396`  
		Last Modified: Fri, 04 Sep 2020 20:11:11 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.8-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:700235b690efc969452c359aa31b2b636e1001730ac02e9d67aec2f035b23370
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6819487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c44b6c5226c848ac88f68fb752a7650eec2ef1ebd3b91fba0e525f5903f7ee3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 04 Sep 2020 19:40:30 GMT
ENV NATS_SERVER=2.1.8
# Fri, 04 Sep 2020 19:40:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='567d5c7f80305b8876230204b993f0cf213411d006d931a036b26dd2288ac81b' ;; 		armhf) natsArch='arm6'; sha256='d76c1ed6f660e13faaa8b1c058723981aa59436ce7d4d4e208ae486395db458f' ;; 		armv7) natsArch='arm7'; sha256='e26f0eba9b065f9537986f88233f279f44c01487aacffe65d4d7440129a5d0a2' ;; 		x86_64) natsArch='amd64'; sha256='8ec25475ef1d49bf5e721de38deb11d689d1a9b2fa588540af78d56cbea2b49d' ;; 		x86) natsArch='386'; sha256='e8535179805573e9d684cc8aa6f79551ab9fcfacd45643d7ba2174e176997d9e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 04 Sep 2020 19:40:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 04 Sep 2020 19:40:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Sep 2020 19:40:36 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:40:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Sep 2020 19:40:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3d1d8b6792cec2b145ec7c0c1b6107e3712804cbd65a93c4d6bc4f5a540ce2`  
		Last Modified: Fri, 04 Sep 2020 19:51:31 GMT  
		Size: 4.1 MB (4094087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c256e59f9e1973a41cd6c2d2af211bfb10c5534b990b63e9c81790cd3c1bdbf3`  
		Last Modified: Fri, 04 Sep 2020 19:51:29 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ea7fd4055fec9b7d9f52d74d616f372dbd367262c3cec827ce3ddc633e3efc`  
		Last Modified: Fri, 04 Sep 2020 19:51:29 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.8-alpine3.11`

```console
$ docker pull nats@sha256:ebe6d1b23a177223608c68d8617049228b00ee54d4e758d2eca44238326b141b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.1.8-alpine3.11` - linux; amd64

```console
$ docker pull nats@sha256:a6f914658a5f8a7a82c9005a3a36863628d331cb2cd4c0c0a3653e7e8a7c0d95
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7208222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96815e17bf1191cbfa7a1745a82f87b8fcc43fbd793da4d66c9fd175c136dd27`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 04 Sep 2020 19:23:32 GMT
ENV NATS_SERVER=2.1.8
# Fri, 04 Sep 2020 19:23:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='567d5c7f80305b8876230204b993f0cf213411d006d931a036b26dd2288ac81b' ;; 		armhf) natsArch='arm6'; sha256='d76c1ed6f660e13faaa8b1c058723981aa59436ce7d4d4e208ae486395db458f' ;; 		armv7) natsArch='arm7'; sha256='e26f0eba9b065f9537986f88233f279f44c01487aacffe65d4d7440129a5d0a2' ;; 		x86_64) natsArch='amd64'; sha256='8ec25475ef1d49bf5e721de38deb11d689d1a9b2fa588540af78d56cbea2b49d' ;; 		x86) natsArch='386'; sha256='e8535179805573e9d684cc8aa6f79551ab9fcfacd45643d7ba2174e176997d9e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 04 Sep 2020 19:23:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 04 Sep 2020 19:23:34 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Sep 2020 19:23:35 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:23:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Sep 2020 19:23:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f9fca7275bd535bd4680297f95f240c9b48d96d0b9b7f17dd38b73917d2b99`  
		Last Modified: Fri, 04 Sep 2020 19:24:56 GMT  
		Size: 4.4 MB (4393961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6905e1079d9ad73fb2f14b529adb1378cfaa4fcabf48ee0a819af4a49842a3a4`  
		Last Modified: Fri, 04 Sep 2020 19:24:55 GMT  
		Size: 530.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a148278ed7ad77a22a36b3ea6e6cdbcaa397edc556440f575992b8bbd8abfc9b`  
		Last Modified: Fri, 04 Sep 2020 19:24:55 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.8-alpine3.11` - linux; arm variant v6

```console
$ docker pull nats@sha256:66672cb8777aa5f85c15c70a90715743fcb7a4b62274bd7ce2a6eae2de23e9f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6736694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3ffd2e3668ab2027e82153bdbc9a30869007677d6a504cf12b55673d415f36f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Sep 2020 20:50:59 GMT
ENV NATS_SERVER=2.1.8
# Tue, 08 Sep 2020 20:51:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='567d5c7f80305b8876230204b993f0cf213411d006d931a036b26dd2288ac81b' ;; 		armhf) natsArch='arm6'; sha256='d76c1ed6f660e13faaa8b1c058723981aa59436ce7d4d4e208ae486395db458f' ;; 		armv7) natsArch='arm7'; sha256='e26f0eba9b065f9537986f88233f279f44c01487aacffe65d4d7440129a5d0a2' ;; 		x86_64) natsArch='amd64'; sha256='8ec25475ef1d49bf5e721de38deb11d689d1a9b2fa588540af78d56cbea2b49d' ;; 		x86) natsArch='386'; sha256='e8535179805573e9d684cc8aa6f79551ab9fcfacd45643d7ba2174e176997d9e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 08 Sep 2020 20:52:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 08 Sep 2020 20:52:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 08 Sep 2020 20:52:29 GMT
EXPOSE 4222 6222 8222
# Tue, 08 Sep 2020 20:52:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 20:52:43 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0ef3723549909739a256c2edd0d1e438f4ecd8eb6a447e818a576156017ba5`  
		Last Modified: Tue, 08 Sep 2020 20:54:21 GMT  
		Size: 4.1 MB (4115782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:495246de42a6ec596d8f30209752a4592e43515a1820cc406d2de5678b60c31b`  
		Last Modified: Tue, 08 Sep 2020 20:54:19 GMT  
		Size: 563.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28539be71de5be5dff99408931259e65df39bb85a070670d75d49f415958062`  
		Last Modified: Tue, 08 Sep 2020 20:54:18 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.8-alpine3.11` - linux; arm variant v7

```console
$ docker pull nats@sha256:645d9707a2e5fbd2330b6b7c87601978add8b5388e18c8a2dc988b2ae00bc7fd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6532999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cbe66195f5f434137dc29427ce470c725a6d3a3fb47451c0608398ec12e0749`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Fri, 04 Sep 2020 20:01:21 GMT
ENV NATS_SERVER=2.1.8
# Fri, 04 Sep 2020 20:01:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='567d5c7f80305b8876230204b993f0cf213411d006d931a036b26dd2288ac81b' ;; 		armhf) natsArch='arm6'; sha256='d76c1ed6f660e13faaa8b1c058723981aa59436ce7d4d4e208ae486395db458f' ;; 		armv7) natsArch='arm7'; sha256='e26f0eba9b065f9537986f88233f279f44c01487aacffe65d4d7440129a5d0a2' ;; 		x86_64) natsArch='amd64'; sha256='8ec25475ef1d49bf5e721de38deb11d689d1a9b2fa588540af78d56cbea2b49d' ;; 		x86) natsArch='386'; sha256='e8535179805573e9d684cc8aa6f79551ab9fcfacd45643d7ba2174e176997d9e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 04 Sep 2020 20:01:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 04 Sep 2020 20:02:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Sep 2020 20:02:18 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 20:02:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Sep 2020 20:02:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707b0a874f39e2d53e2283ffb23bd80599cd3de6fb4813b5d80b6a3576b9a285`  
		Last Modified: Fri, 04 Sep 2020 20:11:13 GMT  
		Size: 4.1 MB (4109958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66cdb37890e6affd51af4e84cb645a7bdca5322a54690e7ed1ef70fd6e7f55b9`  
		Last Modified: Fri, 04 Sep 2020 20:11:11 GMT  
		Size: 562.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358a12bb7b0cdd9809f9bcd5bf1bdbc75c5a232db47e87757596eec47fea3396`  
		Last Modified: Fri, 04 Sep 2020 20:11:11 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.8-alpine3.11` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:700235b690efc969452c359aa31b2b636e1001730ac02e9d67aec2f035b23370
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6819487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c44b6c5226c848ac88f68fb752a7650eec2ef1ebd3b91fba0e525f5903f7ee3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 04 Sep 2020 19:40:30 GMT
ENV NATS_SERVER=2.1.8
# Fri, 04 Sep 2020 19:40:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='567d5c7f80305b8876230204b993f0cf213411d006d931a036b26dd2288ac81b' ;; 		armhf) natsArch='arm6'; sha256='d76c1ed6f660e13faaa8b1c058723981aa59436ce7d4d4e208ae486395db458f' ;; 		armv7) natsArch='arm7'; sha256='e26f0eba9b065f9537986f88233f279f44c01487aacffe65d4d7440129a5d0a2' ;; 		x86_64) natsArch='amd64'; sha256='8ec25475ef1d49bf5e721de38deb11d689d1a9b2fa588540af78d56cbea2b49d' ;; 		x86) natsArch='386'; sha256='e8535179805573e9d684cc8aa6f79551ab9fcfacd45643d7ba2174e176997d9e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 04 Sep 2020 19:40:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 04 Sep 2020 19:40:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Sep 2020 19:40:36 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:40:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Sep 2020 19:40:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3d1d8b6792cec2b145ec7c0c1b6107e3712804cbd65a93c4d6bc4f5a540ce2`  
		Last Modified: Fri, 04 Sep 2020 19:51:31 GMT  
		Size: 4.1 MB (4094087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c256e59f9e1973a41cd6c2d2af211bfb10c5534b990b63e9c81790cd3c1bdbf3`  
		Last Modified: Fri, 04 Sep 2020 19:51:29 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ea7fd4055fec9b7d9f52d74d616f372dbd367262c3cec827ce3ddc633e3efc`  
		Last Modified: Fri, 04 Sep 2020 19:51:29 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.8-linux`

```console
$ docker pull nats@sha256:58f4cc7757a15ffd8f476b74f9d5f199646235b25f85012e759f3cdf64b510a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.1.8-linux` - linux; amd64

```console
$ docker pull nats@sha256:0d7c496dd4f8512bf5c61832bc16e75d805de038fc08554f33fefbcd3907c4b2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4093542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8a33d0935d56b4724ba17d1c68ebc2c6abeab51f35b5c0a9d44bb9749d251c6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 19:24:31 GMT
COPY file:22772fe85f23ca6ef547526020b6f0c57f7bb05cf1b63d4adebc9bac5872d5ce in /nats-server 
# Fri, 04 Sep 2020 19:24:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 19:24:31 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:24:31 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 19:24:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ae9aef3549a0277b3c71f27b28f1616f87abeb4dfcec5ff0f2bb2109fb259b34`  
		Last Modified: Fri, 04 Sep 2020 19:25:04 GMT  
		Size: 4.1 MB (4093066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee674f246b57d546774a96e8caa7a1528c4400b153e22ce806dc1c2cb079a2e9`  
		Last Modified: Fri, 04 Sep 2020 19:25:03 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.8-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:4d7a3526a49cff86b7b08e7754e694bc8debf597effe86c2507fdd4ea32487c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3815178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e62937d0c25fb6d311b12f184e3caa42b65ff2d3988db590064304ff0419db92`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 08 Sep 2020 20:53:16 GMT
COPY file:2414e6a1d4e6c04ea1bd45da76034c284460c92fcf95b5375100eb111f6bcb4f in /nats-server 
# Tue, 08 Sep 2020 20:53:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 08 Sep 2020 20:53:32 GMT
EXPOSE 4222 6222 8222
# Tue, 08 Sep 2020 20:53:37 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 08 Sep 2020 20:53:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:22845e86cdccc8a91bee01c29a4508fa756a18313163373688eadb71457dd1ab`  
		Last Modified: Tue, 08 Sep 2020 20:55:13 GMT  
		Size: 3.8 MB (3814699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048bf9997f96f5831b0b020d70687709d3e7edc8b3cc13fb11363f7bafd6e319`  
		Last Modified: Tue, 08 Sep 2020 20:55:11 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.8-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:20ea87b418a2b1273123ddef4c91956990c5fcab0bbad71523d5b6b434be249c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3811018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0459d9344473c88c51591d37f17b57327d167b6122217d7422431b328c3a1b02`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 20:10:08 GMT
COPY file:3ebd94b1867641b7e927368abdd7734a27a700b6431d3d384660c98fb6f91ae9 in /nats-server 
# Fri, 04 Sep 2020 20:10:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 20:10:26 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 20:10:31 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 20:10:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9388f799ec4c0c97ac0c4f5d9d8936ef881f647ba80558b3f746eea63397a54e`  
		Last Modified: Fri, 04 Sep 2020 20:11:29 GMT  
		Size: 3.8 MB (3810540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce31c20db639568dc0ccc4e73f1bdc208376b2a5b1633adc0587d4ff8aaf0c4`  
		Last Modified: Fri, 04 Sep 2020 20:11:27 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.8-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:46cae43c1deb7bbc919efb2f3271f78e195f1eaa3f8b626376dfdb633ff3b555
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3792562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71a111e279efaf7a4228a57b652684e1adf34e569fc9e077ecd7350dcb0aac50`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 19:51:03 GMT
COPY file:c0962878fe6b8c789e4fa27fcefd32cc868d740092dee272d993d0aac72edeca in /nats-server 
# Fri, 04 Sep 2020 19:51:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 19:51:04 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:51:05 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 19:51:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:176dd0e74c68ca9b537d3cde057424bc8bf3cff7d363d760f1ad421beaef143f`  
		Last Modified: Fri, 04 Sep 2020 19:51:45 GMT  
		Size: 3.8 MB (3792086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b07612acf847f5e6dc42a05a50dbe09be5e7de55f6028a850048895ff39137`  
		Last Modified: Fri, 04 Sep 2020 19:51:44 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.8-nanoserver`

```console
$ docker pull nats@sha256:9e85991423c317f2c30e8cb9c63c064a6afc5225fea43f0b6ac9f1957f24dc48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `nats:2.1.8-nanoserver` - windows version 10.0.17763.1518; amd64

```console
$ docker pull nats@sha256:2bb0cf3737e6f9280c017d9f69a0dd3cc87cd19970c590c82c9bc8a21b465caa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105248098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:784ca74fae547093d5ec6324890b5524d17bab6ec9f6081dd1e10a2b1ebad657`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 30 Sep 2020 11:25:56 GMT
RUN Apply image 1809-amd64
# Wed, 14 Oct 2020 16:26:27 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 16:26:28 GMT
RUN cmd /S /C #(nop) COPY file:0b6475b59bf6bfe6c1030fd41ea501af74fd46ae70fd98c58683b35f8ed498ff in C:\nats-server.exe 
# Wed, 14 Oct 2020 16:26:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Oct 2020 16:26:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Oct 2020 16:26:31 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Oct 2020 16:26:32 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aab6118ce69c93410df7fa15842a6e3b3c7ff20b639c779b5d5f78e7653eaa07`  
		Size: 101.2 MB (101205155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:93b9a3c3e46fc1677426e3be7ce449b91d540c5ae2147380034cc4e1dc7445c3`  
		Last Modified: Wed, 14 Oct 2020 16:31:12 GMT  
		Size: 910.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f192833ce36b0638e48f194ecb14073cd09261d874eb20729671b313f29b3a`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 4.0 MB (4037949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adf949cd79179965570b7d54d6e187eab3a6a5fda1ae9bc15c56233fc001be9`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 1.5 KB (1496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bc641bd835d0a958bbb4a03d9629ffab985d2bde1b52bfeacf45583a784e40`  
		Last Modified: Wed, 14 Oct 2020 16:31:09 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9f9dddc4fec5b66e7c7189d7aa273a6021bfb1c2268ac7cdde04effab31105`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391656292799f8f1ed48dd6d84a3b168cadd87a302f37822617602b6edfa2bbc`  
		Last Modified: Wed, 14 Oct 2020 16:31:14 GMT  
		Size: 865.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.8-nanoserver-1809`

```console
$ docker pull nats@sha256:9e85991423c317f2c30e8cb9c63c064a6afc5225fea43f0b6ac9f1957f24dc48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `nats:2.1.8-nanoserver-1809` - windows version 10.0.17763.1518; amd64

```console
$ docker pull nats@sha256:2bb0cf3737e6f9280c017d9f69a0dd3cc87cd19970c590c82c9bc8a21b465caa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105248098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:784ca74fae547093d5ec6324890b5524d17bab6ec9f6081dd1e10a2b1ebad657`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 30 Sep 2020 11:25:56 GMT
RUN Apply image 1809-amd64
# Wed, 14 Oct 2020 16:26:27 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 16:26:28 GMT
RUN cmd /S /C #(nop) COPY file:0b6475b59bf6bfe6c1030fd41ea501af74fd46ae70fd98c58683b35f8ed498ff in C:\nats-server.exe 
# Wed, 14 Oct 2020 16:26:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Oct 2020 16:26:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Oct 2020 16:26:31 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Oct 2020 16:26:32 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aab6118ce69c93410df7fa15842a6e3b3c7ff20b639c779b5d5f78e7653eaa07`  
		Size: 101.2 MB (101205155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:93b9a3c3e46fc1677426e3be7ce449b91d540c5ae2147380034cc4e1dc7445c3`  
		Last Modified: Wed, 14 Oct 2020 16:31:12 GMT  
		Size: 910.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f192833ce36b0638e48f194ecb14073cd09261d874eb20729671b313f29b3a`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 4.0 MB (4037949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adf949cd79179965570b7d54d6e187eab3a6a5fda1ae9bc15c56233fc001be9`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 1.5 KB (1496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bc641bd835d0a958bbb4a03d9629ffab985d2bde1b52bfeacf45583a784e40`  
		Last Modified: Wed, 14 Oct 2020 16:31:09 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9f9dddc4fec5b66e7c7189d7aa273a6021bfb1c2268ac7cdde04effab31105`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391656292799f8f1ed48dd6d84a3b168cadd87a302f37822617602b6edfa2bbc`  
		Last Modified: Wed, 14 Oct 2020 16:31:14 GMT  
		Size: 865.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.8-scratch`

```console
$ docker pull nats@sha256:58f4cc7757a15ffd8f476b74f9d5f199646235b25f85012e759f3cdf64b510a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.1.8-scratch` - linux; amd64

```console
$ docker pull nats@sha256:0d7c496dd4f8512bf5c61832bc16e75d805de038fc08554f33fefbcd3907c4b2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4093542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8a33d0935d56b4724ba17d1c68ebc2c6abeab51f35b5c0a9d44bb9749d251c6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 19:24:31 GMT
COPY file:22772fe85f23ca6ef547526020b6f0c57f7bb05cf1b63d4adebc9bac5872d5ce in /nats-server 
# Fri, 04 Sep 2020 19:24:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 19:24:31 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:24:31 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 19:24:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ae9aef3549a0277b3c71f27b28f1616f87abeb4dfcec5ff0f2bb2109fb259b34`  
		Last Modified: Fri, 04 Sep 2020 19:25:04 GMT  
		Size: 4.1 MB (4093066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee674f246b57d546774a96e8caa7a1528c4400b153e22ce806dc1c2cb079a2e9`  
		Last Modified: Fri, 04 Sep 2020 19:25:03 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.8-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:4d7a3526a49cff86b7b08e7754e694bc8debf597effe86c2507fdd4ea32487c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3815178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e62937d0c25fb6d311b12f184e3caa42b65ff2d3988db590064304ff0419db92`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 08 Sep 2020 20:53:16 GMT
COPY file:2414e6a1d4e6c04ea1bd45da76034c284460c92fcf95b5375100eb111f6bcb4f in /nats-server 
# Tue, 08 Sep 2020 20:53:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 08 Sep 2020 20:53:32 GMT
EXPOSE 4222 6222 8222
# Tue, 08 Sep 2020 20:53:37 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 08 Sep 2020 20:53:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:22845e86cdccc8a91bee01c29a4508fa756a18313163373688eadb71457dd1ab`  
		Last Modified: Tue, 08 Sep 2020 20:55:13 GMT  
		Size: 3.8 MB (3814699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048bf9997f96f5831b0b020d70687709d3e7edc8b3cc13fb11363f7bafd6e319`  
		Last Modified: Tue, 08 Sep 2020 20:55:11 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.8-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:20ea87b418a2b1273123ddef4c91956990c5fcab0bbad71523d5b6b434be249c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3811018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0459d9344473c88c51591d37f17b57327d167b6122217d7422431b328c3a1b02`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 20:10:08 GMT
COPY file:3ebd94b1867641b7e927368abdd7734a27a700b6431d3d384660c98fb6f91ae9 in /nats-server 
# Fri, 04 Sep 2020 20:10:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 20:10:26 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 20:10:31 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 20:10:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9388f799ec4c0c97ac0c4f5d9d8936ef881f647ba80558b3f746eea63397a54e`  
		Last Modified: Fri, 04 Sep 2020 20:11:29 GMT  
		Size: 3.8 MB (3810540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce31c20db639568dc0ccc4e73f1bdc208376b2a5b1633adc0587d4ff8aaf0c4`  
		Last Modified: Fri, 04 Sep 2020 20:11:27 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.8-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:46cae43c1deb7bbc919efb2f3271f78e195f1eaa3f8b626376dfdb633ff3b555
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3792562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71a111e279efaf7a4228a57b652684e1adf34e569fc9e077ecd7350dcb0aac50`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 19:51:03 GMT
COPY file:c0962878fe6b8c789e4fa27fcefd32cc868d740092dee272d993d0aac72edeca in /nats-server 
# Fri, 04 Sep 2020 19:51:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 19:51:04 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:51:05 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 19:51:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:176dd0e74c68ca9b537d3cde057424bc8bf3cff7d363d760f1ad421beaef143f`  
		Last Modified: Fri, 04 Sep 2020 19:51:45 GMT  
		Size: 3.8 MB (3792086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b07612acf847f5e6dc42a05a50dbe09be5e7de55f6028a850048895ff39137`  
		Last Modified: Fri, 04 Sep 2020 19:51:44 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.8-windowsservercore`

```console
$ docker pull nats@sha256:baa06633b34036a8e5e078f8c852a11d57e8cce09e5069e321afdf065d8ae890
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64
	-	windows version 10.0.14393.3986; amd64

### `nats:2.1.8-windowsservercore` - windows version 10.0.17763.1518; amd64

```console
$ docker pull nats@sha256:39905c59af08a5e40b2d2f0ceae6064a6f9ced58e6621b7822e126cb1756433d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2392178230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c364deb5fbb5c11738060c06fa3616742324103d785e6274055543982212943a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Oct 2020 16:24:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 16:24:31 GMT
ENV NATS_SERVER=2.1.8
# Wed, 14 Oct 2020 16:24:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 14 Oct 2020 16:24:32 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 14 Oct 2020 16:25:04 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Oct 2020 16:26:13 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Oct 2020 16:26:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Oct 2020 16:26:15 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Oct 2020 16:26:16 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Oct 2020 16:26:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d839ec6fa74e5e869036dfd823e95452a7afcde18ac997af483c88c21b92ad8c`  
		Last Modified: Wed, 14 Oct 2020 16:02:33 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad001e4fbf5cfc7ed201221adacaa53c349e1df3803ec7e47dadb618535d55ab`  
		Last Modified: Wed, 14 Oct 2020 16:30:17 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acacbbc13990637bea9cff74311bd0ddfa283dcf6113b3504b190011ffc3fd4d`  
		Last Modified: Wed, 14 Oct 2020 16:30:14 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e9e4a14216f48dde4867109066ee4dc757df1dc14a7efe9f7bce568623f53e`  
		Last Modified: Wed, 14 Oct 2020 16:30:14 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33dbd90143fd1f3cf721c02738e7467399cbdc646bdea4fd8ef2c315a023b5a2`  
		Last Modified: Wed, 14 Oct 2020 16:30:13 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f9eefeebf83c9e54e140cd2009a33d907e6665d183bd564050d0123f4775a7`  
		Last Modified: Wed, 14 Oct 2020 16:30:15 GMT  
		Size: 4.8 MB (4841222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad3755554de955dea91d72362296e93852f543f3a994684fbc5c5eaee5db09c`  
		Last Modified: Wed, 14 Oct 2020 16:30:26 GMT  
		Size: 13.2 MB (13236048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0c72e77ebd4a940053d320e04f69816b175dc2f2580c4a28c9fce89edbc0de`  
		Last Modified: Wed, 14 Oct 2020 16:30:11 GMT  
		Size: 1.7 KB (1697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849395032a9addfec1076fb22ad521b5866c53ff0583299ec6c2c2e401e77626`  
		Last Modified: Wed, 14 Oct 2020 16:30:10 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5be45bbc0b1652484f5e8892f2a886d41255d556a299eb4768a345b75f64eb7`  
		Last Modified: Wed, 14 Oct 2020 16:30:10 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d451d2f47731f173387171f66c25caddbaceb8e9af9ca81dadcf6be5cef98a97`  
		Last Modified: Wed, 14 Oct 2020 16:30:10 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.8-windowsservercore` - windows version 10.0.14393.3986; amd64

```console
$ docker pull nats@sha256:c6745b513657e4cd88add91d5190cd2f436a8656601772df6a93d127cf2dadd8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5760744682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06be644c4b30a273fa9e9ac950062191f85c180f626cecf6304d4b11dd0c2a02`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 13:36:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Oct 2020 16:26:37 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 16:26:38 GMT
ENV NATS_SERVER=2.1.8
# Wed, 14 Oct 2020 16:26:39 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 14 Oct 2020 16:26:39 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 14 Oct 2020 16:27:50 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Oct 2020 16:29:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Oct 2020 16:29:42 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Oct 2020 16:29:43 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Oct 2020 16:29:44 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Oct 2020 16:29:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb0caa156c690c0274404e38041b8eb56dcd2c15edbc269fc4c619eb667cb7ff`  
		Last Modified: Wed, 14 Oct 2020 16:03:09 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abca8ce1a1e304feeddabd9e49e2e5fad5622924c75d97368a7fda9a6eacf3eb`  
		Last Modified: Wed, 14 Oct 2020 16:31:41 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a67950e40a28ee038ef7352f74395d34b51ad95977986eb94b4fc675a66b732`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1adb0de29d8a18a8f87a6be459adb01ad061744c01626323900842810994d9bd`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5759300f31d593f3bafb4b58d462d6980bbafe93c00b2e26f3f7a5009f6183`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d724370e6153197bcd6fcb34163f448999f5086b5b76b726419e2ba8756fab`  
		Last Modified: Wed, 14 Oct 2020 16:31:38 GMT  
		Size: 5.4 MB (5422970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d6803e1700049865bde5e42a043a685787ef6952b6d294169e31a1e7ad0825`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 14.0 MB (13959179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8052312cc55beca318ec095742d503a659b78b71a6a8f711932998a7d312052`  
		Last Modified: Wed, 14 Oct 2020 16:31:34 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac373a9054384aece98f8f7964feb2bc8f8c2c13e692c156e775d6fc4b202927`  
		Last Modified: Wed, 14 Oct 2020 16:31:33 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071d0a2418aea8509bca4632465c04f864b847472a8da8938186f8f4f22ecb6c`  
		Last Modified: Wed, 14 Oct 2020 16:31:34 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b32d70dd6bf96bf57929e861e1ef3ce7d6c9e6037332d4858e8cd4e76f6fba`  
		Last Modified: Wed, 14 Oct 2020 16:31:34 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.8-windowsservercore-1809`

```console
$ docker pull nats@sha256:5cdce689231945e2f25509c3e426374ab5e348f6330f804f83594539aed92425
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `nats:2.1.8-windowsservercore-1809` - windows version 10.0.17763.1518; amd64

```console
$ docker pull nats@sha256:39905c59af08a5e40b2d2f0ceae6064a6f9ced58e6621b7822e126cb1756433d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2392178230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c364deb5fbb5c11738060c06fa3616742324103d785e6274055543982212943a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Oct 2020 16:24:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 16:24:31 GMT
ENV NATS_SERVER=2.1.8
# Wed, 14 Oct 2020 16:24:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 14 Oct 2020 16:24:32 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 14 Oct 2020 16:25:04 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Oct 2020 16:26:13 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Oct 2020 16:26:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Oct 2020 16:26:15 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Oct 2020 16:26:16 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Oct 2020 16:26:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d839ec6fa74e5e869036dfd823e95452a7afcde18ac997af483c88c21b92ad8c`  
		Last Modified: Wed, 14 Oct 2020 16:02:33 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad001e4fbf5cfc7ed201221adacaa53c349e1df3803ec7e47dadb618535d55ab`  
		Last Modified: Wed, 14 Oct 2020 16:30:17 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acacbbc13990637bea9cff74311bd0ddfa283dcf6113b3504b190011ffc3fd4d`  
		Last Modified: Wed, 14 Oct 2020 16:30:14 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e9e4a14216f48dde4867109066ee4dc757df1dc14a7efe9f7bce568623f53e`  
		Last Modified: Wed, 14 Oct 2020 16:30:14 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33dbd90143fd1f3cf721c02738e7467399cbdc646bdea4fd8ef2c315a023b5a2`  
		Last Modified: Wed, 14 Oct 2020 16:30:13 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f9eefeebf83c9e54e140cd2009a33d907e6665d183bd564050d0123f4775a7`  
		Last Modified: Wed, 14 Oct 2020 16:30:15 GMT  
		Size: 4.8 MB (4841222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad3755554de955dea91d72362296e93852f543f3a994684fbc5c5eaee5db09c`  
		Last Modified: Wed, 14 Oct 2020 16:30:26 GMT  
		Size: 13.2 MB (13236048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0c72e77ebd4a940053d320e04f69816b175dc2f2580c4a28c9fce89edbc0de`  
		Last Modified: Wed, 14 Oct 2020 16:30:11 GMT  
		Size: 1.7 KB (1697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849395032a9addfec1076fb22ad521b5866c53ff0583299ec6c2c2e401e77626`  
		Last Modified: Wed, 14 Oct 2020 16:30:10 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5be45bbc0b1652484f5e8892f2a886d41255d556a299eb4768a345b75f64eb7`  
		Last Modified: Wed, 14 Oct 2020 16:30:10 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d451d2f47731f173387171f66c25caddbaceb8e9af9ca81dadcf6be5cef98a97`  
		Last Modified: Wed, 14 Oct 2020 16:30:10 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.8-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:da571ef250c5edb0bc827882ed50510f5544c83ca042f377ca757dd2bdfe13e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3986; amd64

### `nats:2.1.8-windowsservercore-ltsc2016` - windows version 10.0.14393.3986; amd64

```console
$ docker pull nats@sha256:c6745b513657e4cd88add91d5190cd2f436a8656601772df6a93d127cf2dadd8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5760744682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06be644c4b30a273fa9e9ac950062191f85c180f626cecf6304d4b11dd0c2a02`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 13:36:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Oct 2020 16:26:37 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 16:26:38 GMT
ENV NATS_SERVER=2.1.8
# Wed, 14 Oct 2020 16:26:39 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 14 Oct 2020 16:26:39 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 14 Oct 2020 16:27:50 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Oct 2020 16:29:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Oct 2020 16:29:42 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Oct 2020 16:29:43 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Oct 2020 16:29:44 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Oct 2020 16:29:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb0caa156c690c0274404e38041b8eb56dcd2c15edbc269fc4c619eb667cb7ff`  
		Last Modified: Wed, 14 Oct 2020 16:03:09 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abca8ce1a1e304feeddabd9e49e2e5fad5622924c75d97368a7fda9a6eacf3eb`  
		Last Modified: Wed, 14 Oct 2020 16:31:41 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a67950e40a28ee038ef7352f74395d34b51ad95977986eb94b4fc675a66b732`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1adb0de29d8a18a8f87a6be459adb01ad061744c01626323900842810994d9bd`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5759300f31d593f3bafb4b58d462d6980bbafe93c00b2e26f3f7a5009f6183`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d724370e6153197bcd6fcb34163f448999f5086b5b76b726419e2ba8756fab`  
		Last Modified: Wed, 14 Oct 2020 16:31:38 GMT  
		Size: 5.4 MB (5422970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d6803e1700049865bde5e42a043a685787ef6952b6d294169e31a1e7ad0825`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 14.0 MB (13959179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8052312cc55beca318ec095742d503a659b78b71a6a8f711932998a7d312052`  
		Last Modified: Wed, 14 Oct 2020 16:31:34 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac373a9054384aece98f8f7964feb2bc8f8c2c13e692c156e775d6fc4b202927`  
		Last Modified: Wed, 14 Oct 2020 16:31:33 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071d0a2418aea8509bca4632465c04f864b847472a8da8938186f8f4f22ecb6c`  
		Last Modified: Wed, 14 Oct 2020 16:31:34 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b32d70dd6bf96bf57929e861e1ef3ce7d6c9e6037332d4858e8cd4e76f6fba`  
		Last Modified: Wed, 14 Oct 2020 16:31:34 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-alpine`

```console
$ docker pull nats@sha256:ebe6d1b23a177223608c68d8617049228b00ee54d4e758d2eca44238326b141b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.1-alpine` - linux; amd64

```console
$ docker pull nats@sha256:a6f914658a5f8a7a82c9005a3a36863628d331cb2cd4c0c0a3653e7e8a7c0d95
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7208222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96815e17bf1191cbfa7a1745a82f87b8fcc43fbd793da4d66c9fd175c136dd27`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 04 Sep 2020 19:23:32 GMT
ENV NATS_SERVER=2.1.8
# Fri, 04 Sep 2020 19:23:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='567d5c7f80305b8876230204b993f0cf213411d006d931a036b26dd2288ac81b' ;; 		armhf) natsArch='arm6'; sha256='d76c1ed6f660e13faaa8b1c058723981aa59436ce7d4d4e208ae486395db458f' ;; 		armv7) natsArch='arm7'; sha256='e26f0eba9b065f9537986f88233f279f44c01487aacffe65d4d7440129a5d0a2' ;; 		x86_64) natsArch='amd64'; sha256='8ec25475ef1d49bf5e721de38deb11d689d1a9b2fa588540af78d56cbea2b49d' ;; 		x86) natsArch='386'; sha256='e8535179805573e9d684cc8aa6f79551ab9fcfacd45643d7ba2174e176997d9e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 04 Sep 2020 19:23:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 04 Sep 2020 19:23:34 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Sep 2020 19:23:35 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:23:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Sep 2020 19:23:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f9fca7275bd535bd4680297f95f240c9b48d96d0b9b7f17dd38b73917d2b99`  
		Last Modified: Fri, 04 Sep 2020 19:24:56 GMT  
		Size: 4.4 MB (4393961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6905e1079d9ad73fb2f14b529adb1378cfaa4fcabf48ee0a819af4a49842a3a4`  
		Last Modified: Fri, 04 Sep 2020 19:24:55 GMT  
		Size: 530.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a148278ed7ad77a22a36b3ea6e6cdbcaa397edc556440f575992b8bbd8abfc9b`  
		Last Modified: Fri, 04 Sep 2020 19:24:55 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:66672cb8777aa5f85c15c70a90715743fcb7a4b62274bd7ce2a6eae2de23e9f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6736694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3ffd2e3668ab2027e82153bdbc9a30869007677d6a504cf12b55673d415f36f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Sep 2020 20:50:59 GMT
ENV NATS_SERVER=2.1.8
# Tue, 08 Sep 2020 20:51:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='567d5c7f80305b8876230204b993f0cf213411d006d931a036b26dd2288ac81b' ;; 		armhf) natsArch='arm6'; sha256='d76c1ed6f660e13faaa8b1c058723981aa59436ce7d4d4e208ae486395db458f' ;; 		armv7) natsArch='arm7'; sha256='e26f0eba9b065f9537986f88233f279f44c01487aacffe65d4d7440129a5d0a2' ;; 		x86_64) natsArch='amd64'; sha256='8ec25475ef1d49bf5e721de38deb11d689d1a9b2fa588540af78d56cbea2b49d' ;; 		x86) natsArch='386'; sha256='e8535179805573e9d684cc8aa6f79551ab9fcfacd45643d7ba2174e176997d9e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 08 Sep 2020 20:52:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 08 Sep 2020 20:52:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 08 Sep 2020 20:52:29 GMT
EXPOSE 4222 6222 8222
# Tue, 08 Sep 2020 20:52:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 20:52:43 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0ef3723549909739a256c2edd0d1e438f4ecd8eb6a447e818a576156017ba5`  
		Last Modified: Tue, 08 Sep 2020 20:54:21 GMT  
		Size: 4.1 MB (4115782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:495246de42a6ec596d8f30209752a4592e43515a1820cc406d2de5678b60c31b`  
		Last Modified: Tue, 08 Sep 2020 20:54:19 GMT  
		Size: 563.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28539be71de5be5dff99408931259e65df39bb85a070670d75d49f415958062`  
		Last Modified: Tue, 08 Sep 2020 20:54:18 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:645d9707a2e5fbd2330b6b7c87601978add8b5388e18c8a2dc988b2ae00bc7fd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6532999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cbe66195f5f434137dc29427ce470c725a6d3a3fb47451c0608398ec12e0749`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Fri, 04 Sep 2020 20:01:21 GMT
ENV NATS_SERVER=2.1.8
# Fri, 04 Sep 2020 20:01:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='567d5c7f80305b8876230204b993f0cf213411d006d931a036b26dd2288ac81b' ;; 		armhf) natsArch='arm6'; sha256='d76c1ed6f660e13faaa8b1c058723981aa59436ce7d4d4e208ae486395db458f' ;; 		armv7) natsArch='arm7'; sha256='e26f0eba9b065f9537986f88233f279f44c01487aacffe65d4d7440129a5d0a2' ;; 		x86_64) natsArch='amd64'; sha256='8ec25475ef1d49bf5e721de38deb11d689d1a9b2fa588540af78d56cbea2b49d' ;; 		x86) natsArch='386'; sha256='e8535179805573e9d684cc8aa6f79551ab9fcfacd45643d7ba2174e176997d9e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 04 Sep 2020 20:01:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 04 Sep 2020 20:02:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Sep 2020 20:02:18 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 20:02:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Sep 2020 20:02:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707b0a874f39e2d53e2283ffb23bd80599cd3de6fb4813b5d80b6a3576b9a285`  
		Last Modified: Fri, 04 Sep 2020 20:11:13 GMT  
		Size: 4.1 MB (4109958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66cdb37890e6affd51af4e84cb645a7bdca5322a54690e7ed1ef70fd6e7f55b9`  
		Last Modified: Fri, 04 Sep 2020 20:11:11 GMT  
		Size: 562.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358a12bb7b0cdd9809f9bcd5bf1bdbc75c5a232db47e87757596eec47fea3396`  
		Last Modified: Fri, 04 Sep 2020 20:11:11 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:700235b690efc969452c359aa31b2b636e1001730ac02e9d67aec2f035b23370
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6819487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c44b6c5226c848ac88f68fb752a7650eec2ef1ebd3b91fba0e525f5903f7ee3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 04 Sep 2020 19:40:30 GMT
ENV NATS_SERVER=2.1.8
# Fri, 04 Sep 2020 19:40:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='567d5c7f80305b8876230204b993f0cf213411d006d931a036b26dd2288ac81b' ;; 		armhf) natsArch='arm6'; sha256='d76c1ed6f660e13faaa8b1c058723981aa59436ce7d4d4e208ae486395db458f' ;; 		armv7) natsArch='arm7'; sha256='e26f0eba9b065f9537986f88233f279f44c01487aacffe65d4d7440129a5d0a2' ;; 		x86_64) natsArch='amd64'; sha256='8ec25475ef1d49bf5e721de38deb11d689d1a9b2fa588540af78d56cbea2b49d' ;; 		x86) natsArch='386'; sha256='e8535179805573e9d684cc8aa6f79551ab9fcfacd45643d7ba2174e176997d9e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 04 Sep 2020 19:40:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 04 Sep 2020 19:40:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Sep 2020 19:40:36 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:40:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Sep 2020 19:40:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3d1d8b6792cec2b145ec7c0c1b6107e3712804cbd65a93c4d6bc4f5a540ce2`  
		Last Modified: Fri, 04 Sep 2020 19:51:31 GMT  
		Size: 4.1 MB (4094087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c256e59f9e1973a41cd6c2d2af211bfb10c5534b990b63e9c81790cd3c1bdbf3`  
		Last Modified: Fri, 04 Sep 2020 19:51:29 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ea7fd4055fec9b7d9f52d74d616f372dbd367262c3cec827ce3ddc633e3efc`  
		Last Modified: Fri, 04 Sep 2020 19:51:29 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-alpine3.11`

```console
$ docker pull nats@sha256:ebe6d1b23a177223608c68d8617049228b00ee54d4e758d2eca44238326b141b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.1-alpine3.11` - linux; amd64

```console
$ docker pull nats@sha256:a6f914658a5f8a7a82c9005a3a36863628d331cb2cd4c0c0a3653e7e8a7c0d95
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7208222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96815e17bf1191cbfa7a1745a82f87b8fcc43fbd793da4d66c9fd175c136dd27`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 04 Sep 2020 19:23:32 GMT
ENV NATS_SERVER=2.1.8
# Fri, 04 Sep 2020 19:23:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='567d5c7f80305b8876230204b993f0cf213411d006d931a036b26dd2288ac81b' ;; 		armhf) natsArch='arm6'; sha256='d76c1ed6f660e13faaa8b1c058723981aa59436ce7d4d4e208ae486395db458f' ;; 		armv7) natsArch='arm7'; sha256='e26f0eba9b065f9537986f88233f279f44c01487aacffe65d4d7440129a5d0a2' ;; 		x86_64) natsArch='amd64'; sha256='8ec25475ef1d49bf5e721de38deb11d689d1a9b2fa588540af78d56cbea2b49d' ;; 		x86) natsArch='386'; sha256='e8535179805573e9d684cc8aa6f79551ab9fcfacd45643d7ba2174e176997d9e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 04 Sep 2020 19:23:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 04 Sep 2020 19:23:34 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Sep 2020 19:23:35 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:23:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Sep 2020 19:23:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f9fca7275bd535bd4680297f95f240c9b48d96d0b9b7f17dd38b73917d2b99`  
		Last Modified: Fri, 04 Sep 2020 19:24:56 GMT  
		Size: 4.4 MB (4393961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6905e1079d9ad73fb2f14b529adb1378cfaa4fcabf48ee0a819af4a49842a3a4`  
		Last Modified: Fri, 04 Sep 2020 19:24:55 GMT  
		Size: 530.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a148278ed7ad77a22a36b3ea6e6cdbcaa397edc556440f575992b8bbd8abfc9b`  
		Last Modified: Fri, 04 Sep 2020 19:24:55 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-alpine3.11` - linux; arm variant v6

```console
$ docker pull nats@sha256:66672cb8777aa5f85c15c70a90715743fcb7a4b62274bd7ce2a6eae2de23e9f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6736694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3ffd2e3668ab2027e82153bdbc9a30869007677d6a504cf12b55673d415f36f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Sep 2020 20:50:59 GMT
ENV NATS_SERVER=2.1.8
# Tue, 08 Sep 2020 20:51:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='567d5c7f80305b8876230204b993f0cf213411d006d931a036b26dd2288ac81b' ;; 		armhf) natsArch='arm6'; sha256='d76c1ed6f660e13faaa8b1c058723981aa59436ce7d4d4e208ae486395db458f' ;; 		armv7) natsArch='arm7'; sha256='e26f0eba9b065f9537986f88233f279f44c01487aacffe65d4d7440129a5d0a2' ;; 		x86_64) natsArch='amd64'; sha256='8ec25475ef1d49bf5e721de38deb11d689d1a9b2fa588540af78d56cbea2b49d' ;; 		x86) natsArch='386'; sha256='e8535179805573e9d684cc8aa6f79551ab9fcfacd45643d7ba2174e176997d9e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 08 Sep 2020 20:52:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 08 Sep 2020 20:52:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 08 Sep 2020 20:52:29 GMT
EXPOSE 4222 6222 8222
# Tue, 08 Sep 2020 20:52:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 20:52:43 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0ef3723549909739a256c2edd0d1e438f4ecd8eb6a447e818a576156017ba5`  
		Last Modified: Tue, 08 Sep 2020 20:54:21 GMT  
		Size: 4.1 MB (4115782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:495246de42a6ec596d8f30209752a4592e43515a1820cc406d2de5678b60c31b`  
		Last Modified: Tue, 08 Sep 2020 20:54:19 GMT  
		Size: 563.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28539be71de5be5dff99408931259e65df39bb85a070670d75d49f415958062`  
		Last Modified: Tue, 08 Sep 2020 20:54:18 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-alpine3.11` - linux; arm variant v7

```console
$ docker pull nats@sha256:645d9707a2e5fbd2330b6b7c87601978add8b5388e18c8a2dc988b2ae00bc7fd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6532999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cbe66195f5f434137dc29427ce470c725a6d3a3fb47451c0608398ec12e0749`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Fri, 04 Sep 2020 20:01:21 GMT
ENV NATS_SERVER=2.1.8
# Fri, 04 Sep 2020 20:01:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='567d5c7f80305b8876230204b993f0cf213411d006d931a036b26dd2288ac81b' ;; 		armhf) natsArch='arm6'; sha256='d76c1ed6f660e13faaa8b1c058723981aa59436ce7d4d4e208ae486395db458f' ;; 		armv7) natsArch='arm7'; sha256='e26f0eba9b065f9537986f88233f279f44c01487aacffe65d4d7440129a5d0a2' ;; 		x86_64) natsArch='amd64'; sha256='8ec25475ef1d49bf5e721de38deb11d689d1a9b2fa588540af78d56cbea2b49d' ;; 		x86) natsArch='386'; sha256='e8535179805573e9d684cc8aa6f79551ab9fcfacd45643d7ba2174e176997d9e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 04 Sep 2020 20:01:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 04 Sep 2020 20:02:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Sep 2020 20:02:18 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 20:02:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Sep 2020 20:02:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707b0a874f39e2d53e2283ffb23bd80599cd3de6fb4813b5d80b6a3576b9a285`  
		Last Modified: Fri, 04 Sep 2020 20:11:13 GMT  
		Size: 4.1 MB (4109958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66cdb37890e6affd51af4e84cb645a7bdca5322a54690e7ed1ef70fd6e7f55b9`  
		Last Modified: Fri, 04 Sep 2020 20:11:11 GMT  
		Size: 562.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358a12bb7b0cdd9809f9bcd5bf1bdbc75c5a232db47e87757596eec47fea3396`  
		Last Modified: Fri, 04 Sep 2020 20:11:11 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-alpine3.11` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:700235b690efc969452c359aa31b2b636e1001730ac02e9d67aec2f035b23370
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6819487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c44b6c5226c848ac88f68fb752a7650eec2ef1ebd3b91fba0e525f5903f7ee3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 04 Sep 2020 19:40:30 GMT
ENV NATS_SERVER=2.1.8
# Fri, 04 Sep 2020 19:40:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='567d5c7f80305b8876230204b993f0cf213411d006d931a036b26dd2288ac81b' ;; 		armhf) natsArch='arm6'; sha256='d76c1ed6f660e13faaa8b1c058723981aa59436ce7d4d4e208ae486395db458f' ;; 		armv7) natsArch='arm7'; sha256='e26f0eba9b065f9537986f88233f279f44c01487aacffe65d4d7440129a5d0a2' ;; 		x86_64) natsArch='amd64'; sha256='8ec25475ef1d49bf5e721de38deb11d689d1a9b2fa588540af78d56cbea2b49d' ;; 		x86) natsArch='386'; sha256='e8535179805573e9d684cc8aa6f79551ab9fcfacd45643d7ba2174e176997d9e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 04 Sep 2020 19:40:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 04 Sep 2020 19:40:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Sep 2020 19:40:36 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:40:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Sep 2020 19:40:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3d1d8b6792cec2b145ec7c0c1b6107e3712804cbd65a93c4d6bc4f5a540ce2`  
		Last Modified: Fri, 04 Sep 2020 19:51:31 GMT  
		Size: 4.1 MB (4094087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c256e59f9e1973a41cd6c2d2af211bfb10c5534b990b63e9c81790cd3c1bdbf3`  
		Last Modified: Fri, 04 Sep 2020 19:51:29 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ea7fd4055fec9b7d9f52d74d616f372dbd367262c3cec827ce3ddc633e3efc`  
		Last Modified: Fri, 04 Sep 2020 19:51:29 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-linux`

```console
$ docker pull nats@sha256:58f4cc7757a15ffd8f476b74f9d5f199646235b25f85012e759f3cdf64b510a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.1-linux` - linux; amd64

```console
$ docker pull nats@sha256:0d7c496dd4f8512bf5c61832bc16e75d805de038fc08554f33fefbcd3907c4b2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4093542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8a33d0935d56b4724ba17d1c68ebc2c6abeab51f35b5c0a9d44bb9749d251c6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 19:24:31 GMT
COPY file:22772fe85f23ca6ef547526020b6f0c57f7bb05cf1b63d4adebc9bac5872d5ce in /nats-server 
# Fri, 04 Sep 2020 19:24:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 19:24:31 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:24:31 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 19:24:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ae9aef3549a0277b3c71f27b28f1616f87abeb4dfcec5ff0f2bb2109fb259b34`  
		Last Modified: Fri, 04 Sep 2020 19:25:04 GMT  
		Size: 4.1 MB (4093066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee674f246b57d546774a96e8caa7a1528c4400b153e22ce806dc1c2cb079a2e9`  
		Last Modified: Fri, 04 Sep 2020 19:25:03 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:4d7a3526a49cff86b7b08e7754e694bc8debf597effe86c2507fdd4ea32487c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3815178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e62937d0c25fb6d311b12f184e3caa42b65ff2d3988db590064304ff0419db92`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 08 Sep 2020 20:53:16 GMT
COPY file:2414e6a1d4e6c04ea1bd45da76034c284460c92fcf95b5375100eb111f6bcb4f in /nats-server 
# Tue, 08 Sep 2020 20:53:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 08 Sep 2020 20:53:32 GMT
EXPOSE 4222 6222 8222
# Tue, 08 Sep 2020 20:53:37 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 08 Sep 2020 20:53:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:22845e86cdccc8a91bee01c29a4508fa756a18313163373688eadb71457dd1ab`  
		Last Modified: Tue, 08 Sep 2020 20:55:13 GMT  
		Size: 3.8 MB (3814699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048bf9997f96f5831b0b020d70687709d3e7edc8b3cc13fb11363f7bafd6e319`  
		Last Modified: Tue, 08 Sep 2020 20:55:11 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:20ea87b418a2b1273123ddef4c91956990c5fcab0bbad71523d5b6b434be249c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3811018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0459d9344473c88c51591d37f17b57327d167b6122217d7422431b328c3a1b02`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 20:10:08 GMT
COPY file:3ebd94b1867641b7e927368abdd7734a27a700b6431d3d384660c98fb6f91ae9 in /nats-server 
# Fri, 04 Sep 2020 20:10:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 20:10:26 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 20:10:31 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 20:10:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9388f799ec4c0c97ac0c4f5d9d8936ef881f647ba80558b3f746eea63397a54e`  
		Last Modified: Fri, 04 Sep 2020 20:11:29 GMT  
		Size: 3.8 MB (3810540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce31c20db639568dc0ccc4e73f1bdc208376b2a5b1633adc0587d4ff8aaf0c4`  
		Last Modified: Fri, 04 Sep 2020 20:11:27 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:46cae43c1deb7bbc919efb2f3271f78e195f1eaa3f8b626376dfdb633ff3b555
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3792562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71a111e279efaf7a4228a57b652684e1adf34e569fc9e077ecd7350dcb0aac50`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 19:51:03 GMT
COPY file:c0962878fe6b8c789e4fa27fcefd32cc868d740092dee272d993d0aac72edeca in /nats-server 
# Fri, 04 Sep 2020 19:51:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 19:51:04 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:51:05 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 19:51:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:176dd0e74c68ca9b537d3cde057424bc8bf3cff7d363d760f1ad421beaef143f`  
		Last Modified: Fri, 04 Sep 2020 19:51:45 GMT  
		Size: 3.8 MB (3792086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b07612acf847f5e6dc42a05a50dbe09be5e7de55f6028a850048895ff39137`  
		Last Modified: Fri, 04 Sep 2020 19:51:44 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-nanoserver`

```console
$ docker pull nats@sha256:9e85991423c317f2c30e8cb9c63c064a6afc5225fea43f0b6ac9f1957f24dc48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `nats:2.1-nanoserver` - windows version 10.0.17763.1518; amd64

```console
$ docker pull nats@sha256:2bb0cf3737e6f9280c017d9f69a0dd3cc87cd19970c590c82c9bc8a21b465caa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105248098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:784ca74fae547093d5ec6324890b5524d17bab6ec9f6081dd1e10a2b1ebad657`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 30 Sep 2020 11:25:56 GMT
RUN Apply image 1809-amd64
# Wed, 14 Oct 2020 16:26:27 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 16:26:28 GMT
RUN cmd /S /C #(nop) COPY file:0b6475b59bf6bfe6c1030fd41ea501af74fd46ae70fd98c58683b35f8ed498ff in C:\nats-server.exe 
# Wed, 14 Oct 2020 16:26:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Oct 2020 16:26:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Oct 2020 16:26:31 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Oct 2020 16:26:32 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aab6118ce69c93410df7fa15842a6e3b3c7ff20b639c779b5d5f78e7653eaa07`  
		Size: 101.2 MB (101205155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:93b9a3c3e46fc1677426e3be7ce449b91d540c5ae2147380034cc4e1dc7445c3`  
		Last Modified: Wed, 14 Oct 2020 16:31:12 GMT  
		Size: 910.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f192833ce36b0638e48f194ecb14073cd09261d874eb20729671b313f29b3a`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 4.0 MB (4037949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adf949cd79179965570b7d54d6e187eab3a6a5fda1ae9bc15c56233fc001be9`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 1.5 KB (1496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bc641bd835d0a958bbb4a03d9629ffab985d2bde1b52bfeacf45583a784e40`  
		Last Modified: Wed, 14 Oct 2020 16:31:09 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9f9dddc4fec5b66e7c7189d7aa273a6021bfb1c2268ac7cdde04effab31105`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391656292799f8f1ed48dd6d84a3b168cadd87a302f37822617602b6edfa2bbc`  
		Last Modified: Wed, 14 Oct 2020 16:31:14 GMT  
		Size: 865.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-nanoserver-1809`

```console
$ docker pull nats@sha256:9e85991423c317f2c30e8cb9c63c064a6afc5225fea43f0b6ac9f1957f24dc48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `nats:2.1-nanoserver-1809` - windows version 10.0.17763.1518; amd64

```console
$ docker pull nats@sha256:2bb0cf3737e6f9280c017d9f69a0dd3cc87cd19970c590c82c9bc8a21b465caa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105248098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:784ca74fae547093d5ec6324890b5524d17bab6ec9f6081dd1e10a2b1ebad657`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 30 Sep 2020 11:25:56 GMT
RUN Apply image 1809-amd64
# Wed, 14 Oct 2020 16:26:27 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 16:26:28 GMT
RUN cmd /S /C #(nop) COPY file:0b6475b59bf6bfe6c1030fd41ea501af74fd46ae70fd98c58683b35f8ed498ff in C:\nats-server.exe 
# Wed, 14 Oct 2020 16:26:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Oct 2020 16:26:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Oct 2020 16:26:31 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Oct 2020 16:26:32 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aab6118ce69c93410df7fa15842a6e3b3c7ff20b639c779b5d5f78e7653eaa07`  
		Size: 101.2 MB (101205155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:93b9a3c3e46fc1677426e3be7ce449b91d540c5ae2147380034cc4e1dc7445c3`  
		Last Modified: Wed, 14 Oct 2020 16:31:12 GMT  
		Size: 910.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f192833ce36b0638e48f194ecb14073cd09261d874eb20729671b313f29b3a`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 4.0 MB (4037949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adf949cd79179965570b7d54d6e187eab3a6a5fda1ae9bc15c56233fc001be9`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 1.5 KB (1496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bc641bd835d0a958bbb4a03d9629ffab985d2bde1b52bfeacf45583a784e40`  
		Last Modified: Wed, 14 Oct 2020 16:31:09 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9f9dddc4fec5b66e7c7189d7aa273a6021bfb1c2268ac7cdde04effab31105`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391656292799f8f1ed48dd6d84a3b168cadd87a302f37822617602b6edfa2bbc`  
		Last Modified: Wed, 14 Oct 2020 16:31:14 GMT  
		Size: 865.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-scratch`

```console
$ docker pull nats@sha256:58f4cc7757a15ffd8f476b74f9d5f199646235b25f85012e759f3cdf64b510a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.1-scratch` - linux; amd64

```console
$ docker pull nats@sha256:0d7c496dd4f8512bf5c61832bc16e75d805de038fc08554f33fefbcd3907c4b2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4093542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8a33d0935d56b4724ba17d1c68ebc2c6abeab51f35b5c0a9d44bb9749d251c6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 19:24:31 GMT
COPY file:22772fe85f23ca6ef547526020b6f0c57f7bb05cf1b63d4adebc9bac5872d5ce in /nats-server 
# Fri, 04 Sep 2020 19:24:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 19:24:31 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:24:31 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 19:24:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ae9aef3549a0277b3c71f27b28f1616f87abeb4dfcec5ff0f2bb2109fb259b34`  
		Last Modified: Fri, 04 Sep 2020 19:25:04 GMT  
		Size: 4.1 MB (4093066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee674f246b57d546774a96e8caa7a1528c4400b153e22ce806dc1c2cb079a2e9`  
		Last Modified: Fri, 04 Sep 2020 19:25:03 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:4d7a3526a49cff86b7b08e7754e694bc8debf597effe86c2507fdd4ea32487c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3815178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e62937d0c25fb6d311b12f184e3caa42b65ff2d3988db590064304ff0419db92`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 08 Sep 2020 20:53:16 GMT
COPY file:2414e6a1d4e6c04ea1bd45da76034c284460c92fcf95b5375100eb111f6bcb4f in /nats-server 
# Tue, 08 Sep 2020 20:53:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 08 Sep 2020 20:53:32 GMT
EXPOSE 4222 6222 8222
# Tue, 08 Sep 2020 20:53:37 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 08 Sep 2020 20:53:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:22845e86cdccc8a91bee01c29a4508fa756a18313163373688eadb71457dd1ab`  
		Last Modified: Tue, 08 Sep 2020 20:55:13 GMT  
		Size: 3.8 MB (3814699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048bf9997f96f5831b0b020d70687709d3e7edc8b3cc13fb11363f7bafd6e319`  
		Last Modified: Tue, 08 Sep 2020 20:55:11 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:20ea87b418a2b1273123ddef4c91956990c5fcab0bbad71523d5b6b434be249c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3811018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0459d9344473c88c51591d37f17b57327d167b6122217d7422431b328c3a1b02`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 20:10:08 GMT
COPY file:3ebd94b1867641b7e927368abdd7734a27a700b6431d3d384660c98fb6f91ae9 in /nats-server 
# Fri, 04 Sep 2020 20:10:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 20:10:26 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 20:10:31 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 20:10:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9388f799ec4c0c97ac0c4f5d9d8936ef881f647ba80558b3f746eea63397a54e`  
		Last Modified: Fri, 04 Sep 2020 20:11:29 GMT  
		Size: 3.8 MB (3810540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce31c20db639568dc0ccc4e73f1bdc208376b2a5b1633adc0587d4ff8aaf0c4`  
		Last Modified: Fri, 04 Sep 2020 20:11:27 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:46cae43c1deb7bbc919efb2f3271f78e195f1eaa3f8b626376dfdb633ff3b555
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3792562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71a111e279efaf7a4228a57b652684e1adf34e569fc9e077ecd7350dcb0aac50`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 19:51:03 GMT
COPY file:c0962878fe6b8c789e4fa27fcefd32cc868d740092dee272d993d0aac72edeca in /nats-server 
# Fri, 04 Sep 2020 19:51:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 19:51:04 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:51:05 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 19:51:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:176dd0e74c68ca9b537d3cde057424bc8bf3cff7d363d760f1ad421beaef143f`  
		Last Modified: Fri, 04 Sep 2020 19:51:45 GMT  
		Size: 3.8 MB (3792086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b07612acf847f5e6dc42a05a50dbe09be5e7de55f6028a850048895ff39137`  
		Last Modified: Fri, 04 Sep 2020 19:51:44 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-windowsservercore`

```console
$ docker pull nats@sha256:baa06633b34036a8e5e078f8c852a11d57e8cce09e5069e321afdf065d8ae890
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64
	-	windows version 10.0.14393.3986; amd64

### `nats:2.1-windowsservercore` - windows version 10.0.17763.1518; amd64

```console
$ docker pull nats@sha256:39905c59af08a5e40b2d2f0ceae6064a6f9ced58e6621b7822e126cb1756433d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2392178230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c364deb5fbb5c11738060c06fa3616742324103d785e6274055543982212943a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Oct 2020 16:24:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 16:24:31 GMT
ENV NATS_SERVER=2.1.8
# Wed, 14 Oct 2020 16:24:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 14 Oct 2020 16:24:32 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 14 Oct 2020 16:25:04 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Oct 2020 16:26:13 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Oct 2020 16:26:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Oct 2020 16:26:15 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Oct 2020 16:26:16 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Oct 2020 16:26:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d839ec6fa74e5e869036dfd823e95452a7afcde18ac997af483c88c21b92ad8c`  
		Last Modified: Wed, 14 Oct 2020 16:02:33 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad001e4fbf5cfc7ed201221adacaa53c349e1df3803ec7e47dadb618535d55ab`  
		Last Modified: Wed, 14 Oct 2020 16:30:17 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acacbbc13990637bea9cff74311bd0ddfa283dcf6113b3504b190011ffc3fd4d`  
		Last Modified: Wed, 14 Oct 2020 16:30:14 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e9e4a14216f48dde4867109066ee4dc757df1dc14a7efe9f7bce568623f53e`  
		Last Modified: Wed, 14 Oct 2020 16:30:14 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33dbd90143fd1f3cf721c02738e7467399cbdc646bdea4fd8ef2c315a023b5a2`  
		Last Modified: Wed, 14 Oct 2020 16:30:13 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f9eefeebf83c9e54e140cd2009a33d907e6665d183bd564050d0123f4775a7`  
		Last Modified: Wed, 14 Oct 2020 16:30:15 GMT  
		Size: 4.8 MB (4841222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad3755554de955dea91d72362296e93852f543f3a994684fbc5c5eaee5db09c`  
		Last Modified: Wed, 14 Oct 2020 16:30:26 GMT  
		Size: 13.2 MB (13236048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0c72e77ebd4a940053d320e04f69816b175dc2f2580c4a28c9fce89edbc0de`  
		Last Modified: Wed, 14 Oct 2020 16:30:11 GMT  
		Size: 1.7 KB (1697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849395032a9addfec1076fb22ad521b5866c53ff0583299ec6c2c2e401e77626`  
		Last Modified: Wed, 14 Oct 2020 16:30:10 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5be45bbc0b1652484f5e8892f2a886d41255d556a299eb4768a345b75f64eb7`  
		Last Modified: Wed, 14 Oct 2020 16:30:10 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d451d2f47731f173387171f66c25caddbaceb8e9af9ca81dadcf6be5cef98a97`  
		Last Modified: Wed, 14 Oct 2020 16:30:10 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-windowsservercore` - windows version 10.0.14393.3986; amd64

```console
$ docker pull nats@sha256:c6745b513657e4cd88add91d5190cd2f436a8656601772df6a93d127cf2dadd8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5760744682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06be644c4b30a273fa9e9ac950062191f85c180f626cecf6304d4b11dd0c2a02`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 13:36:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Oct 2020 16:26:37 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 16:26:38 GMT
ENV NATS_SERVER=2.1.8
# Wed, 14 Oct 2020 16:26:39 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 14 Oct 2020 16:26:39 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 14 Oct 2020 16:27:50 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Oct 2020 16:29:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Oct 2020 16:29:42 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Oct 2020 16:29:43 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Oct 2020 16:29:44 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Oct 2020 16:29:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb0caa156c690c0274404e38041b8eb56dcd2c15edbc269fc4c619eb667cb7ff`  
		Last Modified: Wed, 14 Oct 2020 16:03:09 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abca8ce1a1e304feeddabd9e49e2e5fad5622924c75d97368a7fda9a6eacf3eb`  
		Last Modified: Wed, 14 Oct 2020 16:31:41 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a67950e40a28ee038ef7352f74395d34b51ad95977986eb94b4fc675a66b732`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1adb0de29d8a18a8f87a6be459adb01ad061744c01626323900842810994d9bd`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5759300f31d593f3bafb4b58d462d6980bbafe93c00b2e26f3f7a5009f6183`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d724370e6153197bcd6fcb34163f448999f5086b5b76b726419e2ba8756fab`  
		Last Modified: Wed, 14 Oct 2020 16:31:38 GMT  
		Size: 5.4 MB (5422970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d6803e1700049865bde5e42a043a685787ef6952b6d294169e31a1e7ad0825`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 14.0 MB (13959179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8052312cc55beca318ec095742d503a659b78b71a6a8f711932998a7d312052`  
		Last Modified: Wed, 14 Oct 2020 16:31:34 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac373a9054384aece98f8f7964feb2bc8f8c2c13e692c156e775d6fc4b202927`  
		Last Modified: Wed, 14 Oct 2020 16:31:33 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071d0a2418aea8509bca4632465c04f864b847472a8da8938186f8f4f22ecb6c`  
		Last Modified: Wed, 14 Oct 2020 16:31:34 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b32d70dd6bf96bf57929e861e1ef3ce7d6c9e6037332d4858e8cd4e76f6fba`  
		Last Modified: Wed, 14 Oct 2020 16:31:34 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-windowsservercore-1809`

```console
$ docker pull nats@sha256:5cdce689231945e2f25509c3e426374ab5e348f6330f804f83594539aed92425
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `nats:2.1-windowsservercore-1809` - windows version 10.0.17763.1518; amd64

```console
$ docker pull nats@sha256:39905c59af08a5e40b2d2f0ceae6064a6f9ced58e6621b7822e126cb1756433d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2392178230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c364deb5fbb5c11738060c06fa3616742324103d785e6274055543982212943a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Oct 2020 16:24:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 16:24:31 GMT
ENV NATS_SERVER=2.1.8
# Wed, 14 Oct 2020 16:24:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 14 Oct 2020 16:24:32 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 14 Oct 2020 16:25:04 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Oct 2020 16:26:13 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Oct 2020 16:26:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Oct 2020 16:26:15 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Oct 2020 16:26:16 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Oct 2020 16:26:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d839ec6fa74e5e869036dfd823e95452a7afcde18ac997af483c88c21b92ad8c`  
		Last Modified: Wed, 14 Oct 2020 16:02:33 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad001e4fbf5cfc7ed201221adacaa53c349e1df3803ec7e47dadb618535d55ab`  
		Last Modified: Wed, 14 Oct 2020 16:30:17 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acacbbc13990637bea9cff74311bd0ddfa283dcf6113b3504b190011ffc3fd4d`  
		Last Modified: Wed, 14 Oct 2020 16:30:14 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e9e4a14216f48dde4867109066ee4dc757df1dc14a7efe9f7bce568623f53e`  
		Last Modified: Wed, 14 Oct 2020 16:30:14 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33dbd90143fd1f3cf721c02738e7467399cbdc646bdea4fd8ef2c315a023b5a2`  
		Last Modified: Wed, 14 Oct 2020 16:30:13 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f9eefeebf83c9e54e140cd2009a33d907e6665d183bd564050d0123f4775a7`  
		Last Modified: Wed, 14 Oct 2020 16:30:15 GMT  
		Size: 4.8 MB (4841222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad3755554de955dea91d72362296e93852f543f3a994684fbc5c5eaee5db09c`  
		Last Modified: Wed, 14 Oct 2020 16:30:26 GMT  
		Size: 13.2 MB (13236048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0c72e77ebd4a940053d320e04f69816b175dc2f2580c4a28c9fce89edbc0de`  
		Last Modified: Wed, 14 Oct 2020 16:30:11 GMT  
		Size: 1.7 KB (1697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849395032a9addfec1076fb22ad521b5866c53ff0583299ec6c2c2e401e77626`  
		Last Modified: Wed, 14 Oct 2020 16:30:10 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5be45bbc0b1652484f5e8892f2a886d41255d556a299eb4768a345b75f64eb7`  
		Last Modified: Wed, 14 Oct 2020 16:30:10 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d451d2f47731f173387171f66c25caddbaceb8e9af9ca81dadcf6be5cef98a97`  
		Last Modified: Wed, 14 Oct 2020 16:30:10 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:da571ef250c5edb0bc827882ed50510f5544c83ca042f377ca757dd2bdfe13e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3986; amd64

### `nats:2.1-windowsservercore-ltsc2016` - windows version 10.0.14393.3986; amd64

```console
$ docker pull nats@sha256:c6745b513657e4cd88add91d5190cd2f436a8656601772df6a93d127cf2dadd8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5760744682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06be644c4b30a273fa9e9ac950062191f85c180f626cecf6304d4b11dd0c2a02`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 13:36:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Oct 2020 16:26:37 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 16:26:38 GMT
ENV NATS_SERVER=2.1.8
# Wed, 14 Oct 2020 16:26:39 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 14 Oct 2020 16:26:39 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 14 Oct 2020 16:27:50 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Oct 2020 16:29:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Oct 2020 16:29:42 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Oct 2020 16:29:43 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Oct 2020 16:29:44 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Oct 2020 16:29:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb0caa156c690c0274404e38041b8eb56dcd2c15edbc269fc4c619eb667cb7ff`  
		Last Modified: Wed, 14 Oct 2020 16:03:09 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abca8ce1a1e304feeddabd9e49e2e5fad5622924c75d97368a7fda9a6eacf3eb`  
		Last Modified: Wed, 14 Oct 2020 16:31:41 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a67950e40a28ee038ef7352f74395d34b51ad95977986eb94b4fc675a66b732`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1adb0de29d8a18a8f87a6be459adb01ad061744c01626323900842810994d9bd`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5759300f31d593f3bafb4b58d462d6980bbafe93c00b2e26f3f7a5009f6183`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d724370e6153197bcd6fcb34163f448999f5086b5b76b726419e2ba8756fab`  
		Last Modified: Wed, 14 Oct 2020 16:31:38 GMT  
		Size: 5.4 MB (5422970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d6803e1700049865bde5e42a043a685787ef6952b6d294169e31a1e7ad0825`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 14.0 MB (13959179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8052312cc55beca318ec095742d503a659b78b71a6a8f711932998a7d312052`  
		Last Modified: Wed, 14 Oct 2020 16:31:34 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac373a9054384aece98f8f7964feb2bc8f8c2c13e692c156e775d6fc4b202927`  
		Last Modified: Wed, 14 Oct 2020 16:31:33 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071d0a2418aea8509bca4632465c04f864b847472a8da8938186f8f4f22ecb6c`  
		Last Modified: Wed, 14 Oct 2020 16:31:34 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b32d70dd6bf96bf57929e861e1ef3ce7d6c9e6037332d4858e8cd4e76f6fba`  
		Last Modified: Wed, 14 Oct 2020 16:31:34 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:ebe6d1b23a177223608c68d8617049228b00ee54d4e758d2eca44238326b141b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:a6f914658a5f8a7a82c9005a3a36863628d331cb2cd4c0c0a3653e7e8a7c0d95
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7208222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96815e17bf1191cbfa7a1745a82f87b8fcc43fbd793da4d66c9fd175c136dd27`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 04 Sep 2020 19:23:32 GMT
ENV NATS_SERVER=2.1.8
# Fri, 04 Sep 2020 19:23:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='567d5c7f80305b8876230204b993f0cf213411d006d931a036b26dd2288ac81b' ;; 		armhf) natsArch='arm6'; sha256='d76c1ed6f660e13faaa8b1c058723981aa59436ce7d4d4e208ae486395db458f' ;; 		armv7) natsArch='arm7'; sha256='e26f0eba9b065f9537986f88233f279f44c01487aacffe65d4d7440129a5d0a2' ;; 		x86_64) natsArch='amd64'; sha256='8ec25475ef1d49bf5e721de38deb11d689d1a9b2fa588540af78d56cbea2b49d' ;; 		x86) natsArch='386'; sha256='e8535179805573e9d684cc8aa6f79551ab9fcfacd45643d7ba2174e176997d9e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 04 Sep 2020 19:23:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 04 Sep 2020 19:23:34 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Sep 2020 19:23:35 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:23:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Sep 2020 19:23:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f9fca7275bd535bd4680297f95f240c9b48d96d0b9b7f17dd38b73917d2b99`  
		Last Modified: Fri, 04 Sep 2020 19:24:56 GMT  
		Size: 4.4 MB (4393961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6905e1079d9ad73fb2f14b529adb1378cfaa4fcabf48ee0a819af4a49842a3a4`  
		Last Modified: Fri, 04 Sep 2020 19:24:55 GMT  
		Size: 530.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a148278ed7ad77a22a36b3ea6e6cdbcaa397edc556440f575992b8bbd8abfc9b`  
		Last Modified: Fri, 04 Sep 2020 19:24:55 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:66672cb8777aa5f85c15c70a90715743fcb7a4b62274bd7ce2a6eae2de23e9f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6736694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3ffd2e3668ab2027e82153bdbc9a30869007677d6a504cf12b55673d415f36f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Sep 2020 20:50:59 GMT
ENV NATS_SERVER=2.1.8
# Tue, 08 Sep 2020 20:51:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='567d5c7f80305b8876230204b993f0cf213411d006d931a036b26dd2288ac81b' ;; 		armhf) natsArch='arm6'; sha256='d76c1ed6f660e13faaa8b1c058723981aa59436ce7d4d4e208ae486395db458f' ;; 		armv7) natsArch='arm7'; sha256='e26f0eba9b065f9537986f88233f279f44c01487aacffe65d4d7440129a5d0a2' ;; 		x86_64) natsArch='amd64'; sha256='8ec25475ef1d49bf5e721de38deb11d689d1a9b2fa588540af78d56cbea2b49d' ;; 		x86) natsArch='386'; sha256='e8535179805573e9d684cc8aa6f79551ab9fcfacd45643d7ba2174e176997d9e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 08 Sep 2020 20:52:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 08 Sep 2020 20:52:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 08 Sep 2020 20:52:29 GMT
EXPOSE 4222 6222 8222
# Tue, 08 Sep 2020 20:52:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 20:52:43 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0ef3723549909739a256c2edd0d1e438f4ecd8eb6a447e818a576156017ba5`  
		Last Modified: Tue, 08 Sep 2020 20:54:21 GMT  
		Size: 4.1 MB (4115782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:495246de42a6ec596d8f30209752a4592e43515a1820cc406d2de5678b60c31b`  
		Last Modified: Tue, 08 Sep 2020 20:54:19 GMT  
		Size: 563.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28539be71de5be5dff99408931259e65df39bb85a070670d75d49f415958062`  
		Last Modified: Tue, 08 Sep 2020 20:54:18 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:645d9707a2e5fbd2330b6b7c87601978add8b5388e18c8a2dc988b2ae00bc7fd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6532999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cbe66195f5f434137dc29427ce470c725a6d3a3fb47451c0608398ec12e0749`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Fri, 04 Sep 2020 20:01:21 GMT
ENV NATS_SERVER=2.1.8
# Fri, 04 Sep 2020 20:01:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='567d5c7f80305b8876230204b993f0cf213411d006d931a036b26dd2288ac81b' ;; 		armhf) natsArch='arm6'; sha256='d76c1ed6f660e13faaa8b1c058723981aa59436ce7d4d4e208ae486395db458f' ;; 		armv7) natsArch='arm7'; sha256='e26f0eba9b065f9537986f88233f279f44c01487aacffe65d4d7440129a5d0a2' ;; 		x86_64) natsArch='amd64'; sha256='8ec25475ef1d49bf5e721de38deb11d689d1a9b2fa588540af78d56cbea2b49d' ;; 		x86) natsArch='386'; sha256='e8535179805573e9d684cc8aa6f79551ab9fcfacd45643d7ba2174e176997d9e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 04 Sep 2020 20:01:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 04 Sep 2020 20:02:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Sep 2020 20:02:18 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 20:02:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Sep 2020 20:02:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707b0a874f39e2d53e2283ffb23bd80599cd3de6fb4813b5d80b6a3576b9a285`  
		Last Modified: Fri, 04 Sep 2020 20:11:13 GMT  
		Size: 4.1 MB (4109958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66cdb37890e6affd51af4e84cb645a7bdca5322a54690e7ed1ef70fd6e7f55b9`  
		Last Modified: Fri, 04 Sep 2020 20:11:11 GMT  
		Size: 562.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358a12bb7b0cdd9809f9bcd5bf1bdbc75c5a232db47e87757596eec47fea3396`  
		Last Modified: Fri, 04 Sep 2020 20:11:11 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:700235b690efc969452c359aa31b2b636e1001730ac02e9d67aec2f035b23370
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6819487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c44b6c5226c848ac88f68fb752a7650eec2ef1ebd3b91fba0e525f5903f7ee3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 04 Sep 2020 19:40:30 GMT
ENV NATS_SERVER=2.1.8
# Fri, 04 Sep 2020 19:40:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='567d5c7f80305b8876230204b993f0cf213411d006d931a036b26dd2288ac81b' ;; 		armhf) natsArch='arm6'; sha256='d76c1ed6f660e13faaa8b1c058723981aa59436ce7d4d4e208ae486395db458f' ;; 		armv7) natsArch='arm7'; sha256='e26f0eba9b065f9537986f88233f279f44c01487aacffe65d4d7440129a5d0a2' ;; 		x86_64) natsArch='amd64'; sha256='8ec25475ef1d49bf5e721de38deb11d689d1a9b2fa588540af78d56cbea2b49d' ;; 		x86) natsArch='386'; sha256='e8535179805573e9d684cc8aa6f79551ab9fcfacd45643d7ba2174e176997d9e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 04 Sep 2020 19:40:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 04 Sep 2020 19:40:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Sep 2020 19:40:36 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:40:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Sep 2020 19:40:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3d1d8b6792cec2b145ec7c0c1b6107e3712804cbd65a93c4d6bc4f5a540ce2`  
		Last Modified: Fri, 04 Sep 2020 19:51:31 GMT  
		Size: 4.1 MB (4094087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c256e59f9e1973a41cd6c2d2af211bfb10c5534b990b63e9c81790cd3c1bdbf3`  
		Last Modified: Fri, 04 Sep 2020 19:51:29 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ea7fd4055fec9b7d9f52d74d616f372dbd367262c3cec827ce3ddc633e3efc`  
		Last Modified: Fri, 04 Sep 2020 19:51:29 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.11`

```console
$ docker pull nats@sha256:ebe6d1b23a177223608c68d8617049228b00ee54d4e758d2eca44238326b141b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.11` - linux; amd64

```console
$ docker pull nats@sha256:a6f914658a5f8a7a82c9005a3a36863628d331cb2cd4c0c0a3653e7e8a7c0d95
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7208222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96815e17bf1191cbfa7a1745a82f87b8fcc43fbd793da4d66c9fd175c136dd27`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 04 Sep 2020 19:23:32 GMT
ENV NATS_SERVER=2.1.8
# Fri, 04 Sep 2020 19:23:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='567d5c7f80305b8876230204b993f0cf213411d006d931a036b26dd2288ac81b' ;; 		armhf) natsArch='arm6'; sha256='d76c1ed6f660e13faaa8b1c058723981aa59436ce7d4d4e208ae486395db458f' ;; 		armv7) natsArch='arm7'; sha256='e26f0eba9b065f9537986f88233f279f44c01487aacffe65d4d7440129a5d0a2' ;; 		x86_64) natsArch='amd64'; sha256='8ec25475ef1d49bf5e721de38deb11d689d1a9b2fa588540af78d56cbea2b49d' ;; 		x86) natsArch='386'; sha256='e8535179805573e9d684cc8aa6f79551ab9fcfacd45643d7ba2174e176997d9e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 04 Sep 2020 19:23:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 04 Sep 2020 19:23:34 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Sep 2020 19:23:35 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:23:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Sep 2020 19:23:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f9fca7275bd535bd4680297f95f240c9b48d96d0b9b7f17dd38b73917d2b99`  
		Last Modified: Fri, 04 Sep 2020 19:24:56 GMT  
		Size: 4.4 MB (4393961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6905e1079d9ad73fb2f14b529adb1378cfaa4fcabf48ee0a819af4a49842a3a4`  
		Last Modified: Fri, 04 Sep 2020 19:24:55 GMT  
		Size: 530.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a148278ed7ad77a22a36b3ea6e6cdbcaa397edc556440f575992b8bbd8abfc9b`  
		Last Modified: Fri, 04 Sep 2020 19:24:55 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.11` - linux; arm variant v6

```console
$ docker pull nats@sha256:66672cb8777aa5f85c15c70a90715743fcb7a4b62274bd7ce2a6eae2de23e9f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6736694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3ffd2e3668ab2027e82153bdbc9a30869007677d6a504cf12b55673d415f36f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Sep 2020 20:50:59 GMT
ENV NATS_SERVER=2.1.8
# Tue, 08 Sep 2020 20:51:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='567d5c7f80305b8876230204b993f0cf213411d006d931a036b26dd2288ac81b' ;; 		armhf) natsArch='arm6'; sha256='d76c1ed6f660e13faaa8b1c058723981aa59436ce7d4d4e208ae486395db458f' ;; 		armv7) natsArch='arm7'; sha256='e26f0eba9b065f9537986f88233f279f44c01487aacffe65d4d7440129a5d0a2' ;; 		x86_64) natsArch='amd64'; sha256='8ec25475ef1d49bf5e721de38deb11d689d1a9b2fa588540af78d56cbea2b49d' ;; 		x86) natsArch='386'; sha256='e8535179805573e9d684cc8aa6f79551ab9fcfacd45643d7ba2174e176997d9e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 08 Sep 2020 20:52:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 08 Sep 2020 20:52:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 08 Sep 2020 20:52:29 GMT
EXPOSE 4222 6222 8222
# Tue, 08 Sep 2020 20:52:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 20:52:43 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0ef3723549909739a256c2edd0d1e438f4ecd8eb6a447e818a576156017ba5`  
		Last Modified: Tue, 08 Sep 2020 20:54:21 GMT  
		Size: 4.1 MB (4115782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:495246de42a6ec596d8f30209752a4592e43515a1820cc406d2de5678b60c31b`  
		Last Modified: Tue, 08 Sep 2020 20:54:19 GMT  
		Size: 563.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28539be71de5be5dff99408931259e65df39bb85a070670d75d49f415958062`  
		Last Modified: Tue, 08 Sep 2020 20:54:18 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.11` - linux; arm variant v7

```console
$ docker pull nats@sha256:645d9707a2e5fbd2330b6b7c87601978add8b5388e18c8a2dc988b2ae00bc7fd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6532999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cbe66195f5f434137dc29427ce470c725a6d3a3fb47451c0608398ec12e0749`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Fri, 04 Sep 2020 20:01:21 GMT
ENV NATS_SERVER=2.1.8
# Fri, 04 Sep 2020 20:01:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='567d5c7f80305b8876230204b993f0cf213411d006d931a036b26dd2288ac81b' ;; 		armhf) natsArch='arm6'; sha256='d76c1ed6f660e13faaa8b1c058723981aa59436ce7d4d4e208ae486395db458f' ;; 		armv7) natsArch='arm7'; sha256='e26f0eba9b065f9537986f88233f279f44c01487aacffe65d4d7440129a5d0a2' ;; 		x86_64) natsArch='amd64'; sha256='8ec25475ef1d49bf5e721de38deb11d689d1a9b2fa588540af78d56cbea2b49d' ;; 		x86) natsArch='386'; sha256='e8535179805573e9d684cc8aa6f79551ab9fcfacd45643d7ba2174e176997d9e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 04 Sep 2020 20:01:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 04 Sep 2020 20:02:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Sep 2020 20:02:18 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 20:02:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Sep 2020 20:02:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707b0a874f39e2d53e2283ffb23bd80599cd3de6fb4813b5d80b6a3576b9a285`  
		Last Modified: Fri, 04 Sep 2020 20:11:13 GMT  
		Size: 4.1 MB (4109958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66cdb37890e6affd51af4e84cb645a7bdca5322a54690e7ed1ef70fd6e7f55b9`  
		Last Modified: Fri, 04 Sep 2020 20:11:11 GMT  
		Size: 562.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358a12bb7b0cdd9809f9bcd5bf1bdbc75c5a232db47e87757596eec47fea3396`  
		Last Modified: Fri, 04 Sep 2020 20:11:11 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.11` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:700235b690efc969452c359aa31b2b636e1001730ac02e9d67aec2f035b23370
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6819487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c44b6c5226c848ac88f68fb752a7650eec2ef1ebd3b91fba0e525f5903f7ee3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 04 Sep 2020 19:40:30 GMT
ENV NATS_SERVER=2.1.8
# Fri, 04 Sep 2020 19:40:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='567d5c7f80305b8876230204b993f0cf213411d006d931a036b26dd2288ac81b' ;; 		armhf) natsArch='arm6'; sha256='d76c1ed6f660e13faaa8b1c058723981aa59436ce7d4d4e208ae486395db458f' ;; 		armv7) natsArch='arm7'; sha256='e26f0eba9b065f9537986f88233f279f44c01487aacffe65d4d7440129a5d0a2' ;; 		x86_64) natsArch='amd64'; sha256='8ec25475ef1d49bf5e721de38deb11d689d1a9b2fa588540af78d56cbea2b49d' ;; 		x86) natsArch='386'; sha256='e8535179805573e9d684cc8aa6f79551ab9fcfacd45643d7ba2174e176997d9e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 04 Sep 2020 19:40:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 04 Sep 2020 19:40:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Sep 2020 19:40:36 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:40:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Sep 2020 19:40:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3d1d8b6792cec2b145ec7c0c1b6107e3712804cbd65a93c4d6bc4f5a540ce2`  
		Last Modified: Fri, 04 Sep 2020 19:51:31 GMT  
		Size: 4.1 MB (4094087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c256e59f9e1973a41cd6c2d2af211bfb10c5534b990b63e9c81790cd3c1bdbf3`  
		Last Modified: Fri, 04 Sep 2020 19:51:29 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ea7fd4055fec9b7d9f52d74d616f372dbd367262c3cec827ce3ddc633e3efc`  
		Last Modified: Fri, 04 Sep 2020 19:51:29 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:58f4cc7757a15ffd8f476b74f9d5f199646235b25f85012e759f3cdf64b510a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:0d7c496dd4f8512bf5c61832bc16e75d805de038fc08554f33fefbcd3907c4b2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4093542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8a33d0935d56b4724ba17d1c68ebc2c6abeab51f35b5c0a9d44bb9749d251c6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 19:24:31 GMT
COPY file:22772fe85f23ca6ef547526020b6f0c57f7bb05cf1b63d4adebc9bac5872d5ce in /nats-server 
# Fri, 04 Sep 2020 19:24:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 19:24:31 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:24:31 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 19:24:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ae9aef3549a0277b3c71f27b28f1616f87abeb4dfcec5ff0f2bb2109fb259b34`  
		Last Modified: Fri, 04 Sep 2020 19:25:04 GMT  
		Size: 4.1 MB (4093066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee674f246b57d546774a96e8caa7a1528c4400b153e22ce806dc1c2cb079a2e9`  
		Last Modified: Fri, 04 Sep 2020 19:25:03 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:4d7a3526a49cff86b7b08e7754e694bc8debf597effe86c2507fdd4ea32487c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3815178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e62937d0c25fb6d311b12f184e3caa42b65ff2d3988db590064304ff0419db92`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 08 Sep 2020 20:53:16 GMT
COPY file:2414e6a1d4e6c04ea1bd45da76034c284460c92fcf95b5375100eb111f6bcb4f in /nats-server 
# Tue, 08 Sep 2020 20:53:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 08 Sep 2020 20:53:32 GMT
EXPOSE 4222 6222 8222
# Tue, 08 Sep 2020 20:53:37 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 08 Sep 2020 20:53:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:22845e86cdccc8a91bee01c29a4508fa756a18313163373688eadb71457dd1ab`  
		Last Modified: Tue, 08 Sep 2020 20:55:13 GMT  
		Size: 3.8 MB (3814699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048bf9997f96f5831b0b020d70687709d3e7edc8b3cc13fb11363f7bafd6e319`  
		Last Modified: Tue, 08 Sep 2020 20:55:11 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:20ea87b418a2b1273123ddef4c91956990c5fcab0bbad71523d5b6b434be249c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3811018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0459d9344473c88c51591d37f17b57327d167b6122217d7422431b328c3a1b02`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 20:10:08 GMT
COPY file:3ebd94b1867641b7e927368abdd7734a27a700b6431d3d384660c98fb6f91ae9 in /nats-server 
# Fri, 04 Sep 2020 20:10:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 20:10:26 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 20:10:31 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 20:10:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9388f799ec4c0c97ac0c4f5d9d8936ef881f647ba80558b3f746eea63397a54e`  
		Last Modified: Fri, 04 Sep 2020 20:11:29 GMT  
		Size: 3.8 MB (3810540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce31c20db639568dc0ccc4e73f1bdc208376b2a5b1633adc0587d4ff8aaf0c4`  
		Last Modified: Fri, 04 Sep 2020 20:11:27 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:46cae43c1deb7bbc919efb2f3271f78e195f1eaa3f8b626376dfdb633ff3b555
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3792562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71a111e279efaf7a4228a57b652684e1adf34e569fc9e077ecd7350dcb0aac50`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 19:51:03 GMT
COPY file:c0962878fe6b8c789e4fa27fcefd32cc868d740092dee272d993d0aac72edeca in /nats-server 
# Fri, 04 Sep 2020 19:51:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 19:51:04 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:51:05 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 19:51:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:176dd0e74c68ca9b537d3cde057424bc8bf3cff7d363d760f1ad421beaef143f`  
		Last Modified: Fri, 04 Sep 2020 19:51:45 GMT  
		Size: 3.8 MB (3792086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b07612acf847f5e6dc42a05a50dbe09be5e7de55f6028a850048895ff39137`  
		Last Modified: Fri, 04 Sep 2020 19:51:44 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:9e85991423c317f2c30e8cb9c63c064a6afc5225fea43f0b6ac9f1957f24dc48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.1518; amd64

```console
$ docker pull nats@sha256:2bb0cf3737e6f9280c017d9f69a0dd3cc87cd19970c590c82c9bc8a21b465caa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105248098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:784ca74fae547093d5ec6324890b5524d17bab6ec9f6081dd1e10a2b1ebad657`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 30 Sep 2020 11:25:56 GMT
RUN Apply image 1809-amd64
# Wed, 14 Oct 2020 16:26:27 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 16:26:28 GMT
RUN cmd /S /C #(nop) COPY file:0b6475b59bf6bfe6c1030fd41ea501af74fd46ae70fd98c58683b35f8ed498ff in C:\nats-server.exe 
# Wed, 14 Oct 2020 16:26:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Oct 2020 16:26:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Oct 2020 16:26:31 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Oct 2020 16:26:32 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aab6118ce69c93410df7fa15842a6e3b3c7ff20b639c779b5d5f78e7653eaa07`  
		Size: 101.2 MB (101205155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:93b9a3c3e46fc1677426e3be7ce449b91d540c5ae2147380034cc4e1dc7445c3`  
		Last Modified: Wed, 14 Oct 2020 16:31:12 GMT  
		Size: 910.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f192833ce36b0638e48f194ecb14073cd09261d874eb20729671b313f29b3a`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 4.0 MB (4037949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adf949cd79179965570b7d54d6e187eab3a6a5fda1ae9bc15c56233fc001be9`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 1.5 KB (1496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bc641bd835d0a958bbb4a03d9629ffab985d2bde1b52bfeacf45583a784e40`  
		Last Modified: Wed, 14 Oct 2020 16:31:09 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9f9dddc4fec5b66e7c7189d7aa273a6021bfb1c2268ac7cdde04effab31105`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391656292799f8f1ed48dd6d84a3b168cadd87a302f37822617602b6edfa2bbc`  
		Last Modified: Wed, 14 Oct 2020 16:31:14 GMT  
		Size: 865.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:9e85991423c317f2c30e8cb9c63c064a6afc5225fea43f0b6ac9f1957f24dc48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.1518; amd64

```console
$ docker pull nats@sha256:2bb0cf3737e6f9280c017d9f69a0dd3cc87cd19970c590c82c9bc8a21b465caa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105248098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:784ca74fae547093d5ec6324890b5524d17bab6ec9f6081dd1e10a2b1ebad657`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 30 Sep 2020 11:25:56 GMT
RUN Apply image 1809-amd64
# Wed, 14 Oct 2020 16:26:27 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 16:26:28 GMT
RUN cmd /S /C #(nop) COPY file:0b6475b59bf6bfe6c1030fd41ea501af74fd46ae70fd98c58683b35f8ed498ff in C:\nats-server.exe 
# Wed, 14 Oct 2020 16:26:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Oct 2020 16:26:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Oct 2020 16:26:31 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Oct 2020 16:26:32 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aab6118ce69c93410df7fa15842a6e3b3c7ff20b639c779b5d5f78e7653eaa07`  
		Size: 101.2 MB (101205155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:93b9a3c3e46fc1677426e3be7ce449b91d540c5ae2147380034cc4e1dc7445c3`  
		Last Modified: Wed, 14 Oct 2020 16:31:12 GMT  
		Size: 910.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f192833ce36b0638e48f194ecb14073cd09261d874eb20729671b313f29b3a`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 4.0 MB (4037949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adf949cd79179965570b7d54d6e187eab3a6a5fda1ae9bc15c56233fc001be9`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 1.5 KB (1496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bc641bd835d0a958bbb4a03d9629ffab985d2bde1b52bfeacf45583a784e40`  
		Last Modified: Wed, 14 Oct 2020 16:31:09 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9f9dddc4fec5b66e7c7189d7aa273a6021bfb1c2268ac7cdde04effab31105`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391656292799f8f1ed48dd6d84a3b168cadd87a302f37822617602b6edfa2bbc`  
		Last Modified: Wed, 14 Oct 2020 16:31:14 GMT  
		Size: 865.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:58f4cc7757a15ffd8f476b74f9d5f199646235b25f85012e759f3cdf64b510a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:0d7c496dd4f8512bf5c61832bc16e75d805de038fc08554f33fefbcd3907c4b2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4093542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8a33d0935d56b4724ba17d1c68ebc2c6abeab51f35b5c0a9d44bb9749d251c6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 19:24:31 GMT
COPY file:22772fe85f23ca6ef547526020b6f0c57f7bb05cf1b63d4adebc9bac5872d5ce in /nats-server 
# Fri, 04 Sep 2020 19:24:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 19:24:31 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:24:31 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 19:24:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ae9aef3549a0277b3c71f27b28f1616f87abeb4dfcec5ff0f2bb2109fb259b34`  
		Last Modified: Fri, 04 Sep 2020 19:25:04 GMT  
		Size: 4.1 MB (4093066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee674f246b57d546774a96e8caa7a1528c4400b153e22ce806dc1c2cb079a2e9`  
		Last Modified: Fri, 04 Sep 2020 19:25:03 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:4d7a3526a49cff86b7b08e7754e694bc8debf597effe86c2507fdd4ea32487c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3815178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e62937d0c25fb6d311b12f184e3caa42b65ff2d3988db590064304ff0419db92`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 08 Sep 2020 20:53:16 GMT
COPY file:2414e6a1d4e6c04ea1bd45da76034c284460c92fcf95b5375100eb111f6bcb4f in /nats-server 
# Tue, 08 Sep 2020 20:53:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 08 Sep 2020 20:53:32 GMT
EXPOSE 4222 6222 8222
# Tue, 08 Sep 2020 20:53:37 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 08 Sep 2020 20:53:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:22845e86cdccc8a91bee01c29a4508fa756a18313163373688eadb71457dd1ab`  
		Last Modified: Tue, 08 Sep 2020 20:55:13 GMT  
		Size: 3.8 MB (3814699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048bf9997f96f5831b0b020d70687709d3e7edc8b3cc13fb11363f7bafd6e319`  
		Last Modified: Tue, 08 Sep 2020 20:55:11 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:20ea87b418a2b1273123ddef4c91956990c5fcab0bbad71523d5b6b434be249c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3811018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0459d9344473c88c51591d37f17b57327d167b6122217d7422431b328c3a1b02`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 20:10:08 GMT
COPY file:3ebd94b1867641b7e927368abdd7734a27a700b6431d3d384660c98fb6f91ae9 in /nats-server 
# Fri, 04 Sep 2020 20:10:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 20:10:26 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 20:10:31 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 20:10:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9388f799ec4c0c97ac0c4f5d9d8936ef881f647ba80558b3f746eea63397a54e`  
		Last Modified: Fri, 04 Sep 2020 20:11:29 GMT  
		Size: 3.8 MB (3810540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce31c20db639568dc0ccc4e73f1bdc208376b2a5b1633adc0587d4ff8aaf0c4`  
		Last Modified: Fri, 04 Sep 2020 20:11:27 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:46cae43c1deb7bbc919efb2f3271f78e195f1eaa3f8b626376dfdb633ff3b555
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3792562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71a111e279efaf7a4228a57b652684e1adf34e569fc9e077ecd7350dcb0aac50`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 19:51:03 GMT
COPY file:c0962878fe6b8c789e4fa27fcefd32cc868d740092dee272d993d0aac72edeca in /nats-server 
# Fri, 04 Sep 2020 19:51:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 19:51:04 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:51:05 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 19:51:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:176dd0e74c68ca9b537d3cde057424bc8bf3cff7d363d760f1ad421beaef143f`  
		Last Modified: Fri, 04 Sep 2020 19:51:45 GMT  
		Size: 3.8 MB (3792086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b07612acf847f5e6dc42a05a50dbe09be5e7de55f6028a850048895ff39137`  
		Last Modified: Fri, 04 Sep 2020 19:51:44 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:baa06633b34036a8e5e078f8c852a11d57e8cce09e5069e321afdf065d8ae890
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64
	-	windows version 10.0.14393.3986; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.1518; amd64

```console
$ docker pull nats@sha256:39905c59af08a5e40b2d2f0ceae6064a6f9ced58e6621b7822e126cb1756433d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2392178230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c364deb5fbb5c11738060c06fa3616742324103d785e6274055543982212943a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Oct 2020 16:24:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 16:24:31 GMT
ENV NATS_SERVER=2.1.8
# Wed, 14 Oct 2020 16:24:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 14 Oct 2020 16:24:32 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 14 Oct 2020 16:25:04 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Oct 2020 16:26:13 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Oct 2020 16:26:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Oct 2020 16:26:15 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Oct 2020 16:26:16 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Oct 2020 16:26:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d839ec6fa74e5e869036dfd823e95452a7afcde18ac997af483c88c21b92ad8c`  
		Last Modified: Wed, 14 Oct 2020 16:02:33 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad001e4fbf5cfc7ed201221adacaa53c349e1df3803ec7e47dadb618535d55ab`  
		Last Modified: Wed, 14 Oct 2020 16:30:17 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acacbbc13990637bea9cff74311bd0ddfa283dcf6113b3504b190011ffc3fd4d`  
		Last Modified: Wed, 14 Oct 2020 16:30:14 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e9e4a14216f48dde4867109066ee4dc757df1dc14a7efe9f7bce568623f53e`  
		Last Modified: Wed, 14 Oct 2020 16:30:14 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33dbd90143fd1f3cf721c02738e7467399cbdc646bdea4fd8ef2c315a023b5a2`  
		Last Modified: Wed, 14 Oct 2020 16:30:13 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f9eefeebf83c9e54e140cd2009a33d907e6665d183bd564050d0123f4775a7`  
		Last Modified: Wed, 14 Oct 2020 16:30:15 GMT  
		Size: 4.8 MB (4841222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad3755554de955dea91d72362296e93852f543f3a994684fbc5c5eaee5db09c`  
		Last Modified: Wed, 14 Oct 2020 16:30:26 GMT  
		Size: 13.2 MB (13236048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0c72e77ebd4a940053d320e04f69816b175dc2f2580c4a28c9fce89edbc0de`  
		Last Modified: Wed, 14 Oct 2020 16:30:11 GMT  
		Size: 1.7 KB (1697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849395032a9addfec1076fb22ad521b5866c53ff0583299ec6c2c2e401e77626`  
		Last Modified: Wed, 14 Oct 2020 16:30:10 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5be45bbc0b1652484f5e8892f2a886d41255d556a299eb4768a345b75f64eb7`  
		Last Modified: Wed, 14 Oct 2020 16:30:10 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d451d2f47731f173387171f66c25caddbaceb8e9af9ca81dadcf6be5cef98a97`  
		Last Modified: Wed, 14 Oct 2020 16:30:10 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.3986; amd64

```console
$ docker pull nats@sha256:c6745b513657e4cd88add91d5190cd2f436a8656601772df6a93d127cf2dadd8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5760744682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06be644c4b30a273fa9e9ac950062191f85c180f626cecf6304d4b11dd0c2a02`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 13:36:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Oct 2020 16:26:37 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 16:26:38 GMT
ENV NATS_SERVER=2.1.8
# Wed, 14 Oct 2020 16:26:39 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 14 Oct 2020 16:26:39 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 14 Oct 2020 16:27:50 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Oct 2020 16:29:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Oct 2020 16:29:42 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Oct 2020 16:29:43 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Oct 2020 16:29:44 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Oct 2020 16:29:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb0caa156c690c0274404e38041b8eb56dcd2c15edbc269fc4c619eb667cb7ff`  
		Last Modified: Wed, 14 Oct 2020 16:03:09 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abca8ce1a1e304feeddabd9e49e2e5fad5622924c75d97368a7fda9a6eacf3eb`  
		Last Modified: Wed, 14 Oct 2020 16:31:41 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a67950e40a28ee038ef7352f74395d34b51ad95977986eb94b4fc675a66b732`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1adb0de29d8a18a8f87a6be459adb01ad061744c01626323900842810994d9bd`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5759300f31d593f3bafb4b58d462d6980bbafe93c00b2e26f3f7a5009f6183`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d724370e6153197bcd6fcb34163f448999f5086b5b76b726419e2ba8756fab`  
		Last Modified: Wed, 14 Oct 2020 16:31:38 GMT  
		Size: 5.4 MB (5422970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d6803e1700049865bde5e42a043a685787ef6952b6d294169e31a1e7ad0825`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 14.0 MB (13959179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8052312cc55beca318ec095742d503a659b78b71a6a8f711932998a7d312052`  
		Last Modified: Wed, 14 Oct 2020 16:31:34 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac373a9054384aece98f8f7964feb2bc8f8c2c13e692c156e775d6fc4b202927`  
		Last Modified: Wed, 14 Oct 2020 16:31:33 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071d0a2418aea8509bca4632465c04f864b847472a8da8938186f8f4f22ecb6c`  
		Last Modified: Wed, 14 Oct 2020 16:31:34 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b32d70dd6bf96bf57929e861e1ef3ce7d6c9e6037332d4858e8cd4e76f6fba`  
		Last Modified: Wed, 14 Oct 2020 16:31:34 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:5cdce689231945e2f25509c3e426374ab5e348f6330f804f83594539aed92425
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.1518; amd64

```console
$ docker pull nats@sha256:39905c59af08a5e40b2d2f0ceae6064a6f9ced58e6621b7822e126cb1756433d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2392178230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c364deb5fbb5c11738060c06fa3616742324103d785e6274055543982212943a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Oct 2020 16:24:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 16:24:31 GMT
ENV NATS_SERVER=2.1.8
# Wed, 14 Oct 2020 16:24:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 14 Oct 2020 16:24:32 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 14 Oct 2020 16:25:04 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Oct 2020 16:26:13 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Oct 2020 16:26:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Oct 2020 16:26:15 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Oct 2020 16:26:16 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Oct 2020 16:26:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d839ec6fa74e5e869036dfd823e95452a7afcde18ac997af483c88c21b92ad8c`  
		Last Modified: Wed, 14 Oct 2020 16:02:33 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad001e4fbf5cfc7ed201221adacaa53c349e1df3803ec7e47dadb618535d55ab`  
		Last Modified: Wed, 14 Oct 2020 16:30:17 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acacbbc13990637bea9cff74311bd0ddfa283dcf6113b3504b190011ffc3fd4d`  
		Last Modified: Wed, 14 Oct 2020 16:30:14 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e9e4a14216f48dde4867109066ee4dc757df1dc14a7efe9f7bce568623f53e`  
		Last Modified: Wed, 14 Oct 2020 16:30:14 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33dbd90143fd1f3cf721c02738e7467399cbdc646bdea4fd8ef2c315a023b5a2`  
		Last Modified: Wed, 14 Oct 2020 16:30:13 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f9eefeebf83c9e54e140cd2009a33d907e6665d183bd564050d0123f4775a7`  
		Last Modified: Wed, 14 Oct 2020 16:30:15 GMT  
		Size: 4.8 MB (4841222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad3755554de955dea91d72362296e93852f543f3a994684fbc5c5eaee5db09c`  
		Last Modified: Wed, 14 Oct 2020 16:30:26 GMT  
		Size: 13.2 MB (13236048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0c72e77ebd4a940053d320e04f69816b175dc2f2580c4a28c9fce89edbc0de`  
		Last Modified: Wed, 14 Oct 2020 16:30:11 GMT  
		Size: 1.7 KB (1697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849395032a9addfec1076fb22ad521b5866c53ff0583299ec6c2c2e401e77626`  
		Last Modified: Wed, 14 Oct 2020 16:30:10 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5be45bbc0b1652484f5e8892f2a886d41255d556a299eb4768a345b75f64eb7`  
		Last Modified: Wed, 14 Oct 2020 16:30:10 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d451d2f47731f173387171f66c25caddbaceb8e9af9ca81dadcf6be5cef98a97`  
		Last Modified: Wed, 14 Oct 2020 16:30:10 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:da571ef250c5edb0bc827882ed50510f5544c83ca042f377ca757dd2bdfe13e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3986; amd64

### `nats:2-windowsservercore-ltsc2016` - windows version 10.0.14393.3986; amd64

```console
$ docker pull nats@sha256:c6745b513657e4cd88add91d5190cd2f436a8656601772df6a93d127cf2dadd8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5760744682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06be644c4b30a273fa9e9ac950062191f85c180f626cecf6304d4b11dd0c2a02`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 13:36:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Oct 2020 16:26:37 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 16:26:38 GMT
ENV NATS_SERVER=2.1.8
# Wed, 14 Oct 2020 16:26:39 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 14 Oct 2020 16:26:39 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 14 Oct 2020 16:27:50 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Oct 2020 16:29:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Oct 2020 16:29:42 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Oct 2020 16:29:43 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Oct 2020 16:29:44 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Oct 2020 16:29:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb0caa156c690c0274404e38041b8eb56dcd2c15edbc269fc4c619eb667cb7ff`  
		Last Modified: Wed, 14 Oct 2020 16:03:09 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abca8ce1a1e304feeddabd9e49e2e5fad5622924c75d97368a7fda9a6eacf3eb`  
		Last Modified: Wed, 14 Oct 2020 16:31:41 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a67950e40a28ee038ef7352f74395d34b51ad95977986eb94b4fc675a66b732`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1adb0de29d8a18a8f87a6be459adb01ad061744c01626323900842810994d9bd`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5759300f31d593f3bafb4b58d462d6980bbafe93c00b2e26f3f7a5009f6183`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d724370e6153197bcd6fcb34163f448999f5086b5b76b726419e2ba8756fab`  
		Last Modified: Wed, 14 Oct 2020 16:31:38 GMT  
		Size: 5.4 MB (5422970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d6803e1700049865bde5e42a043a685787ef6952b6d294169e31a1e7ad0825`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 14.0 MB (13959179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8052312cc55beca318ec095742d503a659b78b71a6a8f711932998a7d312052`  
		Last Modified: Wed, 14 Oct 2020 16:31:34 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac373a9054384aece98f8f7964feb2bc8f8c2c13e692c156e775d6fc4b202927`  
		Last Modified: Wed, 14 Oct 2020 16:31:33 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071d0a2418aea8509bca4632465c04f864b847472a8da8938186f8f4f22ecb6c`  
		Last Modified: Wed, 14 Oct 2020 16:31:34 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b32d70dd6bf96bf57929e861e1ef3ce7d6c9e6037332d4858e8cd4e76f6fba`  
		Last Modified: Wed, 14 Oct 2020 16:31:34 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:ebe6d1b23a177223608c68d8617049228b00ee54d4e758d2eca44238326b141b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:a6f914658a5f8a7a82c9005a3a36863628d331cb2cd4c0c0a3653e7e8a7c0d95
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7208222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96815e17bf1191cbfa7a1745a82f87b8fcc43fbd793da4d66c9fd175c136dd27`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 04 Sep 2020 19:23:32 GMT
ENV NATS_SERVER=2.1.8
# Fri, 04 Sep 2020 19:23:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='567d5c7f80305b8876230204b993f0cf213411d006d931a036b26dd2288ac81b' ;; 		armhf) natsArch='arm6'; sha256='d76c1ed6f660e13faaa8b1c058723981aa59436ce7d4d4e208ae486395db458f' ;; 		armv7) natsArch='arm7'; sha256='e26f0eba9b065f9537986f88233f279f44c01487aacffe65d4d7440129a5d0a2' ;; 		x86_64) natsArch='amd64'; sha256='8ec25475ef1d49bf5e721de38deb11d689d1a9b2fa588540af78d56cbea2b49d' ;; 		x86) natsArch='386'; sha256='e8535179805573e9d684cc8aa6f79551ab9fcfacd45643d7ba2174e176997d9e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 04 Sep 2020 19:23:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 04 Sep 2020 19:23:34 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Sep 2020 19:23:35 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:23:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Sep 2020 19:23:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f9fca7275bd535bd4680297f95f240c9b48d96d0b9b7f17dd38b73917d2b99`  
		Last Modified: Fri, 04 Sep 2020 19:24:56 GMT  
		Size: 4.4 MB (4393961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6905e1079d9ad73fb2f14b529adb1378cfaa4fcabf48ee0a819af4a49842a3a4`  
		Last Modified: Fri, 04 Sep 2020 19:24:55 GMT  
		Size: 530.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a148278ed7ad77a22a36b3ea6e6cdbcaa397edc556440f575992b8bbd8abfc9b`  
		Last Modified: Fri, 04 Sep 2020 19:24:55 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:66672cb8777aa5f85c15c70a90715743fcb7a4b62274bd7ce2a6eae2de23e9f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6736694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3ffd2e3668ab2027e82153bdbc9a30869007677d6a504cf12b55673d415f36f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Sep 2020 20:50:59 GMT
ENV NATS_SERVER=2.1.8
# Tue, 08 Sep 2020 20:51:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='567d5c7f80305b8876230204b993f0cf213411d006d931a036b26dd2288ac81b' ;; 		armhf) natsArch='arm6'; sha256='d76c1ed6f660e13faaa8b1c058723981aa59436ce7d4d4e208ae486395db458f' ;; 		armv7) natsArch='arm7'; sha256='e26f0eba9b065f9537986f88233f279f44c01487aacffe65d4d7440129a5d0a2' ;; 		x86_64) natsArch='amd64'; sha256='8ec25475ef1d49bf5e721de38deb11d689d1a9b2fa588540af78d56cbea2b49d' ;; 		x86) natsArch='386'; sha256='e8535179805573e9d684cc8aa6f79551ab9fcfacd45643d7ba2174e176997d9e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 08 Sep 2020 20:52:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 08 Sep 2020 20:52:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 08 Sep 2020 20:52:29 GMT
EXPOSE 4222 6222 8222
# Tue, 08 Sep 2020 20:52:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 20:52:43 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0ef3723549909739a256c2edd0d1e438f4ecd8eb6a447e818a576156017ba5`  
		Last Modified: Tue, 08 Sep 2020 20:54:21 GMT  
		Size: 4.1 MB (4115782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:495246de42a6ec596d8f30209752a4592e43515a1820cc406d2de5678b60c31b`  
		Last Modified: Tue, 08 Sep 2020 20:54:19 GMT  
		Size: 563.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28539be71de5be5dff99408931259e65df39bb85a070670d75d49f415958062`  
		Last Modified: Tue, 08 Sep 2020 20:54:18 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:645d9707a2e5fbd2330b6b7c87601978add8b5388e18c8a2dc988b2ae00bc7fd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6532999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cbe66195f5f434137dc29427ce470c725a6d3a3fb47451c0608398ec12e0749`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Fri, 04 Sep 2020 20:01:21 GMT
ENV NATS_SERVER=2.1.8
# Fri, 04 Sep 2020 20:01:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='567d5c7f80305b8876230204b993f0cf213411d006d931a036b26dd2288ac81b' ;; 		armhf) natsArch='arm6'; sha256='d76c1ed6f660e13faaa8b1c058723981aa59436ce7d4d4e208ae486395db458f' ;; 		armv7) natsArch='arm7'; sha256='e26f0eba9b065f9537986f88233f279f44c01487aacffe65d4d7440129a5d0a2' ;; 		x86_64) natsArch='amd64'; sha256='8ec25475ef1d49bf5e721de38deb11d689d1a9b2fa588540af78d56cbea2b49d' ;; 		x86) natsArch='386'; sha256='e8535179805573e9d684cc8aa6f79551ab9fcfacd45643d7ba2174e176997d9e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 04 Sep 2020 20:01:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 04 Sep 2020 20:02:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Sep 2020 20:02:18 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 20:02:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Sep 2020 20:02:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707b0a874f39e2d53e2283ffb23bd80599cd3de6fb4813b5d80b6a3576b9a285`  
		Last Modified: Fri, 04 Sep 2020 20:11:13 GMT  
		Size: 4.1 MB (4109958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66cdb37890e6affd51af4e84cb645a7bdca5322a54690e7ed1ef70fd6e7f55b9`  
		Last Modified: Fri, 04 Sep 2020 20:11:11 GMT  
		Size: 562.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358a12bb7b0cdd9809f9bcd5bf1bdbc75c5a232db47e87757596eec47fea3396`  
		Last Modified: Fri, 04 Sep 2020 20:11:11 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:700235b690efc969452c359aa31b2b636e1001730ac02e9d67aec2f035b23370
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6819487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c44b6c5226c848ac88f68fb752a7650eec2ef1ebd3b91fba0e525f5903f7ee3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 04 Sep 2020 19:40:30 GMT
ENV NATS_SERVER=2.1.8
# Fri, 04 Sep 2020 19:40:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='567d5c7f80305b8876230204b993f0cf213411d006d931a036b26dd2288ac81b' ;; 		armhf) natsArch='arm6'; sha256='d76c1ed6f660e13faaa8b1c058723981aa59436ce7d4d4e208ae486395db458f' ;; 		armv7) natsArch='arm7'; sha256='e26f0eba9b065f9537986f88233f279f44c01487aacffe65d4d7440129a5d0a2' ;; 		x86_64) natsArch='amd64'; sha256='8ec25475ef1d49bf5e721de38deb11d689d1a9b2fa588540af78d56cbea2b49d' ;; 		x86) natsArch='386'; sha256='e8535179805573e9d684cc8aa6f79551ab9fcfacd45643d7ba2174e176997d9e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 04 Sep 2020 19:40:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 04 Sep 2020 19:40:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Sep 2020 19:40:36 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:40:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Sep 2020 19:40:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3d1d8b6792cec2b145ec7c0c1b6107e3712804cbd65a93c4d6bc4f5a540ce2`  
		Last Modified: Fri, 04 Sep 2020 19:51:31 GMT  
		Size: 4.1 MB (4094087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c256e59f9e1973a41cd6c2d2af211bfb10c5534b990b63e9c81790cd3c1bdbf3`  
		Last Modified: Fri, 04 Sep 2020 19:51:29 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ea7fd4055fec9b7d9f52d74d616f372dbd367262c3cec827ce3ddc633e3efc`  
		Last Modified: Fri, 04 Sep 2020 19:51:29 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.11`

```console
$ docker pull nats@sha256:ebe6d1b23a177223608c68d8617049228b00ee54d4e758d2eca44238326b141b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.11` - linux; amd64

```console
$ docker pull nats@sha256:a6f914658a5f8a7a82c9005a3a36863628d331cb2cd4c0c0a3653e7e8a7c0d95
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7208222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96815e17bf1191cbfa7a1745a82f87b8fcc43fbd793da4d66c9fd175c136dd27`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 04 Sep 2020 19:23:32 GMT
ENV NATS_SERVER=2.1.8
# Fri, 04 Sep 2020 19:23:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='567d5c7f80305b8876230204b993f0cf213411d006d931a036b26dd2288ac81b' ;; 		armhf) natsArch='arm6'; sha256='d76c1ed6f660e13faaa8b1c058723981aa59436ce7d4d4e208ae486395db458f' ;; 		armv7) natsArch='arm7'; sha256='e26f0eba9b065f9537986f88233f279f44c01487aacffe65d4d7440129a5d0a2' ;; 		x86_64) natsArch='amd64'; sha256='8ec25475ef1d49bf5e721de38deb11d689d1a9b2fa588540af78d56cbea2b49d' ;; 		x86) natsArch='386'; sha256='e8535179805573e9d684cc8aa6f79551ab9fcfacd45643d7ba2174e176997d9e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 04 Sep 2020 19:23:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 04 Sep 2020 19:23:34 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Sep 2020 19:23:35 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:23:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Sep 2020 19:23:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f9fca7275bd535bd4680297f95f240c9b48d96d0b9b7f17dd38b73917d2b99`  
		Last Modified: Fri, 04 Sep 2020 19:24:56 GMT  
		Size: 4.4 MB (4393961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6905e1079d9ad73fb2f14b529adb1378cfaa4fcabf48ee0a819af4a49842a3a4`  
		Last Modified: Fri, 04 Sep 2020 19:24:55 GMT  
		Size: 530.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a148278ed7ad77a22a36b3ea6e6cdbcaa397edc556440f575992b8bbd8abfc9b`  
		Last Modified: Fri, 04 Sep 2020 19:24:55 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.11` - linux; arm variant v6

```console
$ docker pull nats@sha256:66672cb8777aa5f85c15c70a90715743fcb7a4b62274bd7ce2a6eae2de23e9f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6736694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3ffd2e3668ab2027e82153bdbc9a30869007677d6a504cf12b55673d415f36f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Tue, 08 Sep 2020 20:50:59 GMT
ENV NATS_SERVER=2.1.8
# Tue, 08 Sep 2020 20:51:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='567d5c7f80305b8876230204b993f0cf213411d006d931a036b26dd2288ac81b' ;; 		armhf) natsArch='arm6'; sha256='d76c1ed6f660e13faaa8b1c058723981aa59436ce7d4d4e208ae486395db458f' ;; 		armv7) natsArch='arm7'; sha256='e26f0eba9b065f9537986f88233f279f44c01487aacffe65d4d7440129a5d0a2' ;; 		x86_64) natsArch='amd64'; sha256='8ec25475ef1d49bf5e721de38deb11d689d1a9b2fa588540af78d56cbea2b49d' ;; 		x86) natsArch='386'; sha256='e8535179805573e9d684cc8aa6f79551ab9fcfacd45643d7ba2174e176997d9e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 08 Sep 2020 20:52:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 08 Sep 2020 20:52:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 08 Sep 2020 20:52:29 GMT
EXPOSE 4222 6222 8222
# Tue, 08 Sep 2020 20:52:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Sep 2020 20:52:43 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0ef3723549909739a256c2edd0d1e438f4ecd8eb6a447e818a576156017ba5`  
		Last Modified: Tue, 08 Sep 2020 20:54:21 GMT  
		Size: 4.1 MB (4115782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:495246de42a6ec596d8f30209752a4592e43515a1820cc406d2de5678b60c31b`  
		Last Modified: Tue, 08 Sep 2020 20:54:19 GMT  
		Size: 563.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28539be71de5be5dff99408931259e65df39bb85a070670d75d49f415958062`  
		Last Modified: Tue, 08 Sep 2020 20:54:18 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.11` - linux; arm variant v7

```console
$ docker pull nats@sha256:645d9707a2e5fbd2330b6b7c87601978add8b5388e18c8a2dc988b2ae00bc7fd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6532999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cbe66195f5f434137dc29427ce470c725a6d3a3fb47451c0608398ec12e0749`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Fri, 04 Sep 2020 20:01:21 GMT
ENV NATS_SERVER=2.1.8
# Fri, 04 Sep 2020 20:01:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='567d5c7f80305b8876230204b993f0cf213411d006d931a036b26dd2288ac81b' ;; 		armhf) natsArch='arm6'; sha256='d76c1ed6f660e13faaa8b1c058723981aa59436ce7d4d4e208ae486395db458f' ;; 		armv7) natsArch='arm7'; sha256='e26f0eba9b065f9537986f88233f279f44c01487aacffe65d4d7440129a5d0a2' ;; 		x86_64) natsArch='amd64'; sha256='8ec25475ef1d49bf5e721de38deb11d689d1a9b2fa588540af78d56cbea2b49d' ;; 		x86) natsArch='386'; sha256='e8535179805573e9d684cc8aa6f79551ab9fcfacd45643d7ba2174e176997d9e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 04 Sep 2020 20:01:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 04 Sep 2020 20:02:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Sep 2020 20:02:18 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 20:02:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Sep 2020 20:02:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707b0a874f39e2d53e2283ffb23bd80599cd3de6fb4813b5d80b6a3576b9a285`  
		Last Modified: Fri, 04 Sep 2020 20:11:13 GMT  
		Size: 4.1 MB (4109958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66cdb37890e6affd51af4e84cb645a7bdca5322a54690e7ed1ef70fd6e7f55b9`  
		Last Modified: Fri, 04 Sep 2020 20:11:11 GMT  
		Size: 562.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358a12bb7b0cdd9809f9bcd5bf1bdbc75c5a232db47e87757596eec47fea3396`  
		Last Modified: Fri, 04 Sep 2020 20:11:11 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.11` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:700235b690efc969452c359aa31b2b636e1001730ac02e9d67aec2f035b23370
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6819487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c44b6c5226c848ac88f68fb752a7650eec2ef1ebd3b91fba0e525f5903f7ee3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 04 Sep 2020 19:40:30 GMT
ENV NATS_SERVER=2.1.8
# Fri, 04 Sep 2020 19:40:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='567d5c7f80305b8876230204b993f0cf213411d006d931a036b26dd2288ac81b' ;; 		armhf) natsArch='arm6'; sha256='d76c1ed6f660e13faaa8b1c058723981aa59436ce7d4d4e208ae486395db458f' ;; 		armv7) natsArch='arm7'; sha256='e26f0eba9b065f9537986f88233f279f44c01487aacffe65d4d7440129a5d0a2' ;; 		x86_64) natsArch='amd64'; sha256='8ec25475ef1d49bf5e721de38deb11d689d1a9b2fa588540af78d56cbea2b49d' ;; 		x86) natsArch='386'; sha256='e8535179805573e9d684cc8aa6f79551ab9fcfacd45643d7ba2174e176997d9e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 04 Sep 2020 19:40:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 04 Sep 2020 19:40:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Sep 2020 19:40:36 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:40:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Sep 2020 19:40:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3d1d8b6792cec2b145ec7c0c1b6107e3712804cbd65a93c4d6bc4f5a540ce2`  
		Last Modified: Fri, 04 Sep 2020 19:51:31 GMT  
		Size: 4.1 MB (4094087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c256e59f9e1973a41cd6c2d2af211bfb10c5534b990b63e9c81790cd3c1bdbf3`  
		Last Modified: Fri, 04 Sep 2020 19:51:29 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ea7fd4055fec9b7d9f52d74d616f372dbd367262c3cec827ce3ddc633e3efc`  
		Last Modified: Fri, 04 Sep 2020 19:51:29 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:d24378f3491a4ba21c6ec5cddd787f7d4b8004d045ff9fe227037d12491f375e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1518; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:0d7c496dd4f8512bf5c61832bc16e75d805de038fc08554f33fefbcd3907c4b2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4093542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8a33d0935d56b4724ba17d1c68ebc2c6abeab51f35b5c0a9d44bb9749d251c6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 19:24:31 GMT
COPY file:22772fe85f23ca6ef547526020b6f0c57f7bb05cf1b63d4adebc9bac5872d5ce in /nats-server 
# Fri, 04 Sep 2020 19:24:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 19:24:31 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:24:31 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 19:24:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ae9aef3549a0277b3c71f27b28f1616f87abeb4dfcec5ff0f2bb2109fb259b34`  
		Last Modified: Fri, 04 Sep 2020 19:25:04 GMT  
		Size: 4.1 MB (4093066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee674f246b57d546774a96e8caa7a1528c4400b153e22ce806dc1c2cb079a2e9`  
		Last Modified: Fri, 04 Sep 2020 19:25:03 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:4d7a3526a49cff86b7b08e7754e694bc8debf597effe86c2507fdd4ea32487c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3815178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e62937d0c25fb6d311b12f184e3caa42b65ff2d3988db590064304ff0419db92`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 08 Sep 2020 20:53:16 GMT
COPY file:2414e6a1d4e6c04ea1bd45da76034c284460c92fcf95b5375100eb111f6bcb4f in /nats-server 
# Tue, 08 Sep 2020 20:53:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 08 Sep 2020 20:53:32 GMT
EXPOSE 4222 6222 8222
# Tue, 08 Sep 2020 20:53:37 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 08 Sep 2020 20:53:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:22845e86cdccc8a91bee01c29a4508fa756a18313163373688eadb71457dd1ab`  
		Last Modified: Tue, 08 Sep 2020 20:55:13 GMT  
		Size: 3.8 MB (3814699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048bf9997f96f5831b0b020d70687709d3e7edc8b3cc13fb11363f7bafd6e319`  
		Last Modified: Tue, 08 Sep 2020 20:55:11 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:20ea87b418a2b1273123ddef4c91956990c5fcab0bbad71523d5b6b434be249c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3811018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0459d9344473c88c51591d37f17b57327d167b6122217d7422431b328c3a1b02`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 20:10:08 GMT
COPY file:3ebd94b1867641b7e927368abdd7734a27a700b6431d3d384660c98fb6f91ae9 in /nats-server 
# Fri, 04 Sep 2020 20:10:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 20:10:26 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 20:10:31 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 20:10:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9388f799ec4c0c97ac0c4f5d9d8936ef881f647ba80558b3f746eea63397a54e`  
		Last Modified: Fri, 04 Sep 2020 20:11:29 GMT  
		Size: 3.8 MB (3810540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce31c20db639568dc0ccc4e73f1bdc208376b2a5b1633adc0587d4ff8aaf0c4`  
		Last Modified: Fri, 04 Sep 2020 20:11:27 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:46cae43c1deb7bbc919efb2f3271f78e195f1eaa3f8b626376dfdb633ff3b555
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3792562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71a111e279efaf7a4228a57b652684e1adf34e569fc9e077ecd7350dcb0aac50`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 19:51:03 GMT
COPY file:c0962878fe6b8c789e4fa27fcefd32cc868d740092dee272d993d0aac72edeca in /nats-server 
# Fri, 04 Sep 2020 19:51:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 19:51:04 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:51:05 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 19:51:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:176dd0e74c68ca9b537d3cde057424bc8bf3cff7d363d760f1ad421beaef143f`  
		Last Modified: Fri, 04 Sep 2020 19:51:45 GMT  
		Size: 3.8 MB (3792086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b07612acf847f5e6dc42a05a50dbe09be5e7de55f6028a850048895ff39137`  
		Last Modified: Fri, 04 Sep 2020 19:51:44 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.1518; amd64

```console
$ docker pull nats@sha256:2bb0cf3737e6f9280c017d9f69a0dd3cc87cd19970c590c82c9bc8a21b465caa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105248098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:784ca74fae547093d5ec6324890b5524d17bab6ec9f6081dd1e10a2b1ebad657`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 30 Sep 2020 11:25:56 GMT
RUN Apply image 1809-amd64
# Wed, 14 Oct 2020 16:26:27 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 16:26:28 GMT
RUN cmd /S /C #(nop) COPY file:0b6475b59bf6bfe6c1030fd41ea501af74fd46ae70fd98c58683b35f8ed498ff in C:\nats-server.exe 
# Wed, 14 Oct 2020 16:26:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Oct 2020 16:26:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Oct 2020 16:26:31 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Oct 2020 16:26:32 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aab6118ce69c93410df7fa15842a6e3b3c7ff20b639c779b5d5f78e7653eaa07`  
		Size: 101.2 MB (101205155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:93b9a3c3e46fc1677426e3be7ce449b91d540c5ae2147380034cc4e1dc7445c3`  
		Last Modified: Wed, 14 Oct 2020 16:31:12 GMT  
		Size: 910.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f192833ce36b0638e48f194ecb14073cd09261d874eb20729671b313f29b3a`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 4.0 MB (4037949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adf949cd79179965570b7d54d6e187eab3a6a5fda1ae9bc15c56233fc001be9`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 1.5 KB (1496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bc641bd835d0a958bbb4a03d9629ffab985d2bde1b52bfeacf45583a784e40`  
		Last Modified: Wed, 14 Oct 2020 16:31:09 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9f9dddc4fec5b66e7c7189d7aa273a6021bfb1c2268ac7cdde04effab31105`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391656292799f8f1ed48dd6d84a3b168cadd87a302f37822617602b6edfa2bbc`  
		Last Modified: Wed, 14 Oct 2020 16:31:14 GMT  
		Size: 865.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:58f4cc7757a15ffd8f476b74f9d5f199646235b25f85012e759f3cdf64b510a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:0d7c496dd4f8512bf5c61832bc16e75d805de038fc08554f33fefbcd3907c4b2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4093542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8a33d0935d56b4724ba17d1c68ebc2c6abeab51f35b5c0a9d44bb9749d251c6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 19:24:31 GMT
COPY file:22772fe85f23ca6ef547526020b6f0c57f7bb05cf1b63d4adebc9bac5872d5ce in /nats-server 
# Fri, 04 Sep 2020 19:24:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 19:24:31 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:24:31 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 19:24:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ae9aef3549a0277b3c71f27b28f1616f87abeb4dfcec5ff0f2bb2109fb259b34`  
		Last Modified: Fri, 04 Sep 2020 19:25:04 GMT  
		Size: 4.1 MB (4093066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee674f246b57d546774a96e8caa7a1528c4400b153e22ce806dc1c2cb079a2e9`  
		Last Modified: Fri, 04 Sep 2020 19:25:03 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:4d7a3526a49cff86b7b08e7754e694bc8debf597effe86c2507fdd4ea32487c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3815178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e62937d0c25fb6d311b12f184e3caa42b65ff2d3988db590064304ff0419db92`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 08 Sep 2020 20:53:16 GMT
COPY file:2414e6a1d4e6c04ea1bd45da76034c284460c92fcf95b5375100eb111f6bcb4f in /nats-server 
# Tue, 08 Sep 2020 20:53:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 08 Sep 2020 20:53:32 GMT
EXPOSE 4222 6222 8222
# Tue, 08 Sep 2020 20:53:37 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 08 Sep 2020 20:53:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:22845e86cdccc8a91bee01c29a4508fa756a18313163373688eadb71457dd1ab`  
		Last Modified: Tue, 08 Sep 2020 20:55:13 GMT  
		Size: 3.8 MB (3814699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048bf9997f96f5831b0b020d70687709d3e7edc8b3cc13fb11363f7bafd6e319`  
		Last Modified: Tue, 08 Sep 2020 20:55:11 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:20ea87b418a2b1273123ddef4c91956990c5fcab0bbad71523d5b6b434be249c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3811018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0459d9344473c88c51591d37f17b57327d167b6122217d7422431b328c3a1b02`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 20:10:08 GMT
COPY file:3ebd94b1867641b7e927368abdd7734a27a700b6431d3d384660c98fb6f91ae9 in /nats-server 
# Fri, 04 Sep 2020 20:10:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 20:10:26 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 20:10:31 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 20:10:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9388f799ec4c0c97ac0c4f5d9d8936ef881f647ba80558b3f746eea63397a54e`  
		Last Modified: Fri, 04 Sep 2020 20:11:29 GMT  
		Size: 3.8 MB (3810540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce31c20db639568dc0ccc4e73f1bdc208376b2a5b1633adc0587d4ff8aaf0c4`  
		Last Modified: Fri, 04 Sep 2020 20:11:27 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:46cae43c1deb7bbc919efb2f3271f78e195f1eaa3f8b626376dfdb633ff3b555
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3792562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71a111e279efaf7a4228a57b652684e1adf34e569fc9e077ecd7350dcb0aac50`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 19:51:03 GMT
COPY file:c0962878fe6b8c789e4fa27fcefd32cc868d740092dee272d993d0aac72edeca in /nats-server 
# Fri, 04 Sep 2020 19:51:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 19:51:04 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:51:05 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 19:51:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:176dd0e74c68ca9b537d3cde057424bc8bf3cff7d363d760f1ad421beaef143f`  
		Last Modified: Fri, 04 Sep 2020 19:51:45 GMT  
		Size: 3.8 MB (3792086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b07612acf847f5e6dc42a05a50dbe09be5e7de55f6028a850048895ff39137`  
		Last Modified: Fri, 04 Sep 2020 19:51:44 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:9e85991423c317f2c30e8cb9c63c064a6afc5225fea43f0b6ac9f1957f24dc48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `nats:nanoserver` - windows version 10.0.17763.1518; amd64

```console
$ docker pull nats@sha256:2bb0cf3737e6f9280c017d9f69a0dd3cc87cd19970c590c82c9bc8a21b465caa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105248098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:784ca74fae547093d5ec6324890b5524d17bab6ec9f6081dd1e10a2b1ebad657`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 30 Sep 2020 11:25:56 GMT
RUN Apply image 1809-amd64
# Wed, 14 Oct 2020 16:26:27 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 16:26:28 GMT
RUN cmd /S /C #(nop) COPY file:0b6475b59bf6bfe6c1030fd41ea501af74fd46ae70fd98c58683b35f8ed498ff in C:\nats-server.exe 
# Wed, 14 Oct 2020 16:26:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Oct 2020 16:26:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Oct 2020 16:26:31 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Oct 2020 16:26:32 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aab6118ce69c93410df7fa15842a6e3b3c7ff20b639c779b5d5f78e7653eaa07`  
		Size: 101.2 MB (101205155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:93b9a3c3e46fc1677426e3be7ce449b91d540c5ae2147380034cc4e1dc7445c3`  
		Last Modified: Wed, 14 Oct 2020 16:31:12 GMT  
		Size: 910.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f192833ce36b0638e48f194ecb14073cd09261d874eb20729671b313f29b3a`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 4.0 MB (4037949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adf949cd79179965570b7d54d6e187eab3a6a5fda1ae9bc15c56233fc001be9`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 1.5 KB (1496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bc641bd835d0a958bbb4a03d9629ffab985d2bde1b52bfeacf45583a784e40`  
		Last Modified: Wed, 14 Oct 2020 16:31:09 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9f9dddc4fec5b66e7c7189d7aa273a6021bfb1c2268ac7cdde04effab31105`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391656292799f8f1ed48dd6d84a3b168cadd87a302f37822617602b6edfa2bbc`  
		Last Modified: Wed, 14 Oct 2020 16:31:14 GMT  
		Size: 865.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:9e85991423c317f2c30e8cb9c63c064a6afc5225fea43f0b6ac9f1957f24dc48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.1518; amd64

```console
$ docker pull nats@sha256:2bb0cf3737e6f9280c017d9f69a0dd3cc87cd19970c590c82c9bc8a21b465caa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105248098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:784ca74fae547093d5ec6324890b5524d17bab6ec9f6081dd1e10a2b1ebad657`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 30 Sep 2020 11:25:56 GMT
RUN Apply image 1809-amd64
# Wed, 14 Oct 2020 16:26:27 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 16:26:28 GMT
RUN cmd /S /C #(nop) COPY file:0b6475b59bf6bfe6c1030fd41ea501af74fd46ae70fd98c58683b35f8ed498ff in C:\nats-server.exe 
# Wed, 14 Oct 2020 16:26:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Oct 2020 16:26:30 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Oct 2020 16:26:31 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Oct 2020 16:26:32 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aab6118ce69c93410df7fa15842a6e3b3c7ff20b639c779b5d5f78e7653eaa07`  
		Size: 101.2 MB (101205155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:93b9a3c3e46fc1677426e3be7ce449b91d540c5ae2147380034cc4e1dc7445c3`  
		Last Modified: Wed, 14 Oct 2020 16:31:12 GMT  
		Size: 910.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f192833ce36b0638e48f194ecb14073cd09261d874eb20729671b313f29b3a`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 4.0 MB (4037949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adf949cd79179965570b7d54d6e187eab3a6a5fda1ae9bc15c56233fc001be9`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 1.5 KB (1496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33bc641bd835d0a958bbb4a03d9629ffab985d2bde1b52bfeacf45583a784e40`  
		Last Modified: Wed, 14 Oct 2020 16:31:09 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9f9dddc4fec5b66e7c7189d7aa273a6021bfb1c2268ac7cdde04effab31105`  
		Last Modified: Wed, 14 Oct 2020 16:31:10 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391656292799f8f1ed48dd6d84a3b168cadd87a302f37822617602b6edfa2bbc`  
		Last Modified: Wed, 14 Oct 2020 16:31:14 GMT  
		Size: 865.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:58f4cc7757a15ffd8f476b74f9d5f199646235b25f85012e759f3cdf64b510a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:0d7c496dd4f8512bf5c61832bc16e75d805de038fc08554f33fefbcd3907c4b2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4093542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8a33d0935d56b4724ba17d1c68ebc2c6abeab51f35b5c0a9d44bb9749d251c6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 19:24:31 GMT
COPY file:22772fe85f23ca6ef547526020b6f0c57f7bb05cf1b63d4adebc9bac5872d5ce in /nats-server 
# Fri, 04 Sep 2020 19:24:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 19:24:31 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:24:31 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 19:24:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ae9aef3549a0277b3c71f27b28f1616f87abeb4dfcec5ff0f2bb2109fb259b34`  
		Last Modified: Fri, 04 Sep 2020 19:25:04 GMT  
		Size: 4.1 MB (4093066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee674f246b57d546774a96e8caa7a1528c4400b153e22ce806dc1c2cb079a2e9`  
		Last Modified: Fri, 04 Sep 2020 19:25:03 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:4d7a3526a49cff86b7b08e7754e694bc8debf597effe86c2507fdd4ea32487c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3815178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e62937d0c25fb6d311b12f184e3caa42b65ff2d3988db590064304ff0419db92`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 08 Sep 2020 20:53:16 GMT
COPY file:2414e6a1d4e6c04ea1bd45da76034c284460c92fcf95b5375100eb111f6bcb4f in /nats-server 
# Tue, 08 Sep 2020 20:53:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 08 Sep 2020 20:53:32 GMT
EXPOSE 4222 6222 8222
# Tue, 08 Sep 2020 20:53:37 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 08 Sep 2020 20:53:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:22845e86cdccc8a91bee01c29a4508fa756a18313163373688eadb71457dd1ab`  
		Last Modified: Tue, 08 Sep 2020 20:55:13 GMT  
		Size: 3.8 MB (3814699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048bf9997f96f5831b0b020d70687709d3e7edc8b3cc13fb11363f7bafd6e319`  
		Last Modified: Tue, 08 Sep 2020 20:55:11 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:20ea87b418a2b1273123ddef4c91956990c5fcab0bbad71523d5b6b434be249c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3811018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0459d9344473c88c51591d37f17b57327d167b6122217d7422431b328c3a1b02`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 20:10:08 GMT
COPY file:3ebd94b1867641b7e927368abdd7734a27a700b6431d3d384660c98fb6f91ae9 in /nats-server 
# Fri, 04 Sep 2020 20:10:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 20:10:26 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 20:10:31 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 20:10:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9388f799ec4c0c97ac0c4f5d9d8936ef881f647ba80558b3f746eea63397a54e`  
		Last Modified: Fri, 04 Sep 2020 20:11:29 GMT  
		Size: 3.8 MB (3810540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce31c20db639568dc0ccc4e73f1bdc208376b2a5b1633adc0587d4ff8aaf0c4`  
		Last Modified: Fri, 04 Sep 2020 20:11:27 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:46cae43c1deb7bbc919efb2f3271f78e195f1eaa3f8b626376dfdb633ff3b555
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3792562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71a111e279efaf7a4228a57b652684e1adf34e569fc9e077ecd7350dcb0aac50`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Sep 2020 19:51:03 GMT
COPY file:c0962878fe6b8c789e4fa27fcefd32cc868d740092dee272d993d0aac72edeca in /nats-server 
# Fri, 04 Sep 2020 19:51:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 04 Sep 2020 19:51:04 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:51:05 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Sep 2020 19:51:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:176dd0e74c68ca9b537d3cde057424bc8bf3cff7d363d760f1ad421beaef143f`  
		Last Modified: Fri, 04 Sep 2020 19:51:45 GMT  
		Size: 3.8 MB (3792086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b07612acf847f5e6dc42a05a50dbe09be5e7de55f6028a850048895ff39137`  
		Last Modified: Fri, 04 Sep 2020 19:51:44 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:baa06633b34036a8e5e078f8c852a11d57e8cce09e5069e321afdf065d8ae890
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64
	-	windows version 10.0.14393.3986; amd64

### `nats:windowsservercore` - windows version 10.0.17763.1518; amd64

```console
$ docker pull nats@sha256:39905c59af08a5e40b2d2f0ceae6064a6f9ced58e6621b7822e126cb1756433d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2392178230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c364deb5fbb5c11738060c06fa3616742324103d785e6274055543982212943a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Oct 2020 16:24:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 16:24:31 GMT
ENV NATS_SERVER=2.1.8
# Wed, 14 Oct 2020 16:24:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 14 Oct 2020 16:24:32 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 14 Oct 2020 16:25:04 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Oct 2020 16:26:13 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Oct 2020 16:26:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Oct 2020 16:26:15 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Oct 2020 16:26:16 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Oct 2020 16:26:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d839ec6fa74e5e869036dfd823e95452a7afcde18ac997af483c88c21b92ad8c`  
		Last Modified: Wed, 14 Oct 2020 16:02:33 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad001e4fbf5cfc7ed201221adacaa53c349e1df3803ec7e47dadb618535d55ab`  
		Last Modified: Wed, 14 Oct 2020 16:30:17 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acacbbc13990637bea9cff74311bd0ddfa283dcf6113b3504b190011ffc3fd4d`  
		Last Modified: Wed, 14 Oct 2020 16:30:14 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e9e4a14216f48dde4867109066ee4dc757df1dc14a7efe9f7bce568623f53e`  
		Last Modified: Wed, 14 Oct 2020 16:30:14 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33dbd90143fd1f3cf721c02738e7467399cbdc646bdea4fd8ef2c315a023b5a2`  
		Last Modified: Wed, 14 Oct 2020 16:30:13 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f9eefeebf83c9e54e140cd2009a33d907e6665d183bd564050d0123f4775a7`  
		Last Modified: Wed, 14 Oct 2020 16:30:15 GMT  
		Size: 4.8 MB (4841222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad3755554de955dea91d72362296e93852f543f3a994684fbc5c5eaee5db09c`  
		Last Modified: Wed, 14 Oct 2020 16:30:26 GMT  
		Size: 13.2 MB (13236048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0c72e77ebd4a940053d320e04f69816b175dc2f2580c4a28c9fce89edbc0de`  
		Last Modified: Wed, 14 Oct 2020 16:30:11 GMT  
		Size: 1.7 KB (1697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849395032a9addfec1076fb22ad521b5866c53ff0583299ec6c2c2e401e77626`  
		Last Modified: Wed, 14 Oct 2020 16:30:10 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5be45bbc0b1652484f5e8892f2a886d41255d556a299eb4768a345b75f64eb7`  
		Last Modified: Wed, 14 Oct 2020 16:30:10 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d451d2f47731f173387171f66c25caddbaceb8e9af9ca81dadcf6be5cef98a97`  
		Last Modified: Wed, 14 Oct 2020 16:30:10 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:windowsservercore` - windows version 10.0.14393.3986; amd64

```console
$ docker pull nats@sha256:c6745b513657e4cd88add91d5190cd2f436a8656601772df6a93d127cf2dadd8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5760744682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06be644c4b30a273fa9e9ac950062191f85c180f626cecf6304d4b11dd0c2a02`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 13:36:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Oct 2020 16:26:37 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 16:26:38 GMT
ENV NATS_SERVER=2.1.8
# Wed, 14 Oct 2020 16:26:39 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 14 Oct 2020 16:26:39 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 14 Oct 2020 16:27:50 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Oct 2020 16:29:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Oct 2020 16:29:42 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Oct 2020 16:29:43 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Oct 2020 16:29:44 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Oct 2020 16:29:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb0caa156c690c0274404e38041b8eb56dcd2c15edbc269fc4c619eb667cb7ff`  
		Last Modified: Wed, 14 Oct 2020 16:03:09 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abca8ce1a1e304feeddabd9e49e2e5fad5622924c75d97368a7fda9a6eacf3eb`  
		Last Modified: Wed, 14 Oct 2020 16:31:41 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a67950e40a28ee038ef7352f74395d34b51ad95977986eb94b4fc675a66b732`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1adb0de29d8a18a8f87a6be459adb01ad061744c01626323900842810994d9bd`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5759300f31d593f3bafb4b58d462d6980bbafe93c00b2e26f3f7a5009f6183`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d724370e6153197bcd6fcb34163f448999f5086b5b76b726419e2ba8756fab`  
		Last Modified: Wed, 14 Oct 2020 16:31:38 GMT  
		Size: 5.4 MB (5422970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d6803e1700049865bde5e42a043a685787ef6952b6d294169e31a1e7ad0825`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 14.0 MB (13959179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8052312cc55beca318ec095742d503a659b78b71a6a8f711932998a7d312052`  
		Last Modified: Wed, 14 Oct 2020 16:31:34 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac373a9054384aece98f8f7964feb2bc8f8c2c13e692c156e775d6fc4b202927`  
		Last Modified: Wed, 14 Oct 2020 16:31:33 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071d0a2418aea8509bca4632465c04f864b847472a8da8938186f8f4f22ecb6c`  
		Last Modified: Wed, 14 Oct 2020 16:31:34 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b32d70dd6bf96bf57929e861e1ef3ce7d6c9e6037332d4858e8cd4e76f6fba`  
		Last Modified: Wed, 14 Oct 2020 16:31:34 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:5cdce689231945e2f25509c3e426374ab5e348f6330f804f83594539aed92425
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.1518; amd64

```console
$ docker pull nats@sha256:39905c59af08a5e40b2d2f0ceae6064a6f9ced58e6621b7822e126cb1756433d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2392178230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c364deb5fbb5c11738060c06fa3616742324103d785e6274055543982212943a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Oct 2020 16:24:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 16:24:31 GMT
ENV NATS_SERVER=2.1.8
# Wed, 14 Oct 2020 16:24:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 14 Oct 2020 16:24:32 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 14 Oct 2020 16:25:04 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Oct 2020 16:26:13 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Oct 2020 16:26:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Oct 2020 16:26:15 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Oct 2020 16:26:16 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Oct 2020 16:26:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d839ec6fa74e5e869036dfd823e95452a7afcde18ac997af483c88c21b92ad8c`  
		Last Modified: Wed, 14 Oct 2020 16:02:33 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad001e4fbf5cfc7ed201221adacaa53c349e1df3803ec7e47dadb618535d55ab`  
		Last Modified: Wed, 14 Oct 2020 16:30:17 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acacbbc13990637bea9cff74311bd0ddfa283dcf6113b3504b190011ffc3fd4d`  
		Last Modified: Wed, 14 Oct 2020 16:30:14 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e9e4a14216f48dde4867109066ee4dc757df1dc14a7efe9f7bce568623f53e`  
		Last Modified: Wed, 14 Oct 2020 16:30:14 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33dbd90143fd1f3cf721c02738e7467399cbdc646bdea4fd8ef2c315a023b5a2`  
		Last Modified: Wed, 14 Oct 2020 16:30:13 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f9eefeebf83c9e54e140cd2009a33d907e6665d183bd564050d0123f4775a7`  
		Last Modified: Wed, 14 Oct 2020 16:30:15 GMT  
		Size: 4.8 MB (4841222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad3755554de955dea91d72362296e93852f543f3a994684fbc5c5eaee5db09c`  
		Last Modified: Wed, 14 Oct 2020 16:30:26 GMT  
		Size: 13.2 MB (13236048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0c72e77ebd4a940053d320e04f69816b175dc2f2580c4a28c9fce89edbc0de`  
		Last Modified: Wed, 14 Oct 2020 16:30:11 GMT  
		Size: 1.7 KB (1697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849395032a9addfec1076fb22ad521b5866c53ff0583299ec6c2c2e401e77626`  
		Last Modified: Wed, 14 Oct 2020 16:30:10 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5be45bbc0b1652484f5e8892f2a886d41255d556a299eb4768a345b75f64eb7`  
		Last Modified: Wed, 14 Oct 2020 16:30:10 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d451d2f47731f173387171f66c25caddbaceb8e9af9ca81dadcf6be5cef98a97`  
		Last Modified: Wed, 14 Oct 2020 16:30:10 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:da571ef250c5edb0bc827882ed50510f5544c83ca042f377ca757dd2bdfe13e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3986; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.3986; amd64

```console
$ docker pull nats@sha256:c6745b513657e4cd88add91d5190cd2f436a8656601772df6a93d127cf2dadd8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5760744682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06be644c4b30a273fa9e9ac950062191f85c180f626cecf6304d4b11dd0c2a02`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 13:36:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Oct 2020 16:26:37 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Oct 2020 16:26:38 GMT
ENV NATS_SERVER=2.1.8
# Wed, 14 Oct 2020 16:26:39 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 14 Oct 2020 16:26:39 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 14 Oct 2020 16:27:50 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Oct 2020 16:29:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Oct 2020 16:29:42 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 14 Oct 2020 16:29:43 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Oct 2020 16:29:44 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Oct 2020 16:29:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb0caa156c690c0274404e38041b8eb56dcd2c15edbc269fc4c619eb667cb7ff`  
		Last Modified: Wed, 14 Oct 2020 16:03:09 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abca8ce1a1e304feeddabd9e49e2e5fad5622924c75d97368a7fda9a6eacf3eb`  
		Last Modified: Wed, 14 Oct 2020 16:31:41 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a67950e40a28ee038ef7352f74395d34b51ad95977986eb94b4fc675a66b732`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1adb0de29d8a18a8f87a6be459adb01ad061744c01626323900842810994d9bd`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5759300f31d593f3bafb4b58d462d6980bbafe93c00b2e26f3f7a5009f6183`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d724370e6153197bcd6fcb34163f448999f5086b5b76b726419e2ba8756fab`  
		Last Modified: Wed, 14 Oct 2020 16:31:38 GMT  
		Size: 5.4 MB (5422970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d6803e1700049865bde5e42a043a685787ef6952b6d294169e31a1e7ad0825`  
		Last Modified: Wed, 14 Oct 2020 16:31:37 GMT  
		Size: 14.0 MB (13959179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8052312cc55beca318ec095742d503a659b78b71a6a8f711932998a7d312052`  
		Last Modified: Wed, 14 Oct 2020 16:31:34 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac373a9054384aece98f8f7964feb2bc8f8c2c13e692c156e775d6fc4b202927`  
		Last Modified: Wed, 14 Oct 2020 16:31:33 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071d0a2418aea8509bca4632465c04f864b847472a8da8938186f8f4f22ecb6c`  
		Last Modified: Wed, 14 Oct 2020 16:31:34 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b32d70dd6bf96bf57929e861e1ef3ce7d6c9e6037332d4858e8cd4e76f6fba`  
		Last Modified: Wed, 14 Oct 2020 16:31:34 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
