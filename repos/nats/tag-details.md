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
$ docker pull nats@sha256:8ef9f9514ee044da7c405a5e2520771f0d1f5ad741246bb0f82a329278e0cb77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1457; amd64

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

### `nats:2` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats@sha256:f4f74a489fc4190ec1f80cfd0c51e63462ccdbe6da88eb8e817106bb4c734469
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.3 MB (105282104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23265cf7e8f5821431c1b7add8531891db26bdc7bfd497a674244d5bfd37e21a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Sep 2020 12:08:18 GMT
RUN Apply image 1809-amd64
# Wed, 09 Sep 2020 17:12:30 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 17:12:32 GMT
RUN cmd /S /C #(nop) COPY file:0b6475b59bf6bfe6c1030fd41ea501af74fd46ae70fd98c58683b35f8ed498ff in C:\nats-server.exe 
# Wed, 09 Sep 2020 17:12:33 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Sep 2020 17:12:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Sep 2020 17:12:34 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Sep 2020 17:12:35 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ecf9bb62dc6eedea9fd367628f8715dea75b7d2053afa4b5121e7809aa692139`  
		Size: 101.2 MB (101239122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a993e00682bb4be271d74c200e8e9d454b07999d7ab172f3b14fe72883380722`  
		Last Modified: Wed, 09 Sep 2020 17:16:30 GMT  
		Size: 929.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2582374a52a2ff5b9749c0da3753f314eebed73312c429dedd53254e3439381`  
		Last Modified: Wed, 09 Sep 2020 17:16:31 GMT  
		Size: 4.0 MB (4037991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1ddaa896f4f824bc34f5423c4a584085484ad6726210c5e85deb31b96dcecf`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 1.5 KB (1473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1c9a98b8493177510bd243f069f3169cf0575b5dbaeccaed59ec06115e30a1`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2065dc75ba87a95592c8d5d558eafa92ac761f14b53075fbf4baf04f30b1c6`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023bb1ddc2afbcca6549888de223caebd1fdb23f9744ddde1ab091e60b0c505e`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1`

```console
$ docker pull nats@sha256:8ef9f9514ee044da7c405a5e2520771f0d1f5ad741246bb0f82a329278e0cb77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1457; amd64

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

### `nats:2.1` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats@sha256:f4f74a489fc4190ec1f80cfd0c51e63462ccdbe6da88eb8e817106bb4c734469
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.3 MB (105282104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23265cf7e8f5821431c1b7add8531891db26bdc7bfd497a674244d5bfd37e21a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Sep 2020 12:08:18 GMT
RUN Apply image 1809-amd64
# Wed, 09 Sep 2020 17:12:30 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 17:12:32 GMT
RUN cmd /S /C #(nop) COPY file:0b6475b59bf6bfe6c1030fd41ea501af74fd46ae70fd98c58683b35f8ed498ff in C:\nats-server.exe 
# Wed, 09 Sep 2020 17:12:33 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Sep 2020 17:12:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Sep 2020 17:12:34 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Sep 2020 17:12:35 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ecf9bb62dc6eedea9fd367628f8715dea75b7d2053afa4b5121e7809aa692139`  
		Size: 101.2 MB (101239122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a993e00682bb4be271d74c200e8e9d454b07999d7ab172f3b14fe72883380722`  
		Last Modified: Wed, 09 Sep 2020 17:16:30 GMT  
		Size: 929.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2582374a52a2ff5b9749c0da3753f314eebed73312c429dedd53254e3439381`  
		Last Modified: Wed, 09 Sep 2020 17:16:31 GMT  
		Size: 4.0 MB (4037991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1ddaa896f4f824bc34f5423c4a584085484ad6726210c5e85deb31b96dcecf`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 1.5 KB (1473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1c9a98b8493177510bd243f069f3169cf0575b5dbaeccaed59ec06115e30a1`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2065dc75ba87a95592c8d5d558eafa92ac761f14b53075fbf4baf04f30b1c6`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023bb1ddc2afbcca6549888de223caebd1fdb23f9744ddde1ab091e60b0c505e`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.8`

```console
$ docker pull nats@sha256:8ef9f9514ee044da7c405a5e2520771f0d1f5ad741246bb0f82a329278e0cb77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1457; amd64

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

### `nats:2.1.8` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats@sha256:f4f74a489fc4190ec1f80cfd0c51e63462ccdbe6da88eb8e817106bb4c734469
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.3 MB (105282104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23265cf7e8f5821431c1b7add8531891db26bdc7bfd497a674244d5bfd37e21a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Sep 2020 12:08:18 GMT
RUN Apply image 1809-amd64
# Wed, 09 Sep 2020 17:12:30 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 17:12:32 GMT
RUN cmd /S /C #(nop) COPY file:0b6475b59bf6bfe6c1030fd41ea501af74fd46ae70fd98c58683b35f8ed498ff in C:\nats-server.exe 
# Wed, 09 Sep 2020 17:12:33 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Sep 2020 17:12:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Sep 2020 17:12:34 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Sep 2020 17:12:35 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ecf9bb62dc6eedea9fd367628f8715dea75b7d2053afa4b5121e7809aa692139`  
		Size: 101.2 MB (101239122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a993e00682bb4be271d74c200e8e9d454b07999d7ab172f3b14fe72883380722`  
		Last Modified: Wed, 09 Sep 2020 17:16:30 GMT  
		Size: 929.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2582374a52a2ff5b9749c0da3753f314eebed73312c429dedd53254e3439381`  
		Last Modified: Wed, 09 Sep 2020 17:16:31 GMT  
		Size: 4.0 MB (4037991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1ddaa896f4f824bc34f5423c4a584085484ad6726210c5e85deb31b96dcecf`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 1.5 KB (1473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1c9a98b8493177510bd243f069f3169cf0575b5dbaeccaed59ec06115e30a1`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2065dc75ba87a95592c8d5d558eafa92ac761f14b53075fbf4baf04f30b1c6`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023bb1ddc2afbcca6549888de223caebd1fdb23f9744ddde1ab091e60b0c505e`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 860.0 B  
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
$ docker pull nats@sha256:43a61a1fde7c2a6eb37e1ca9f9fc62c070d499448ba952313e7e4455be147fbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `nats:2.1.8-nanoserver` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats@sha256:f4f74a489fc4190ec1f80cfd0c51e63462ccdbe6da88eb8e817106bb4c734469
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.3 MB (105282104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23265cf7e8f5821431c1b7add8531891db26bdc7bfd497a674244d5bfd37e21a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Sep 2020 12:08:18 GMT
RUN Apply image 1809-amd64
# Wed, 09 Sep 2020 17:12:30 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 17:12:32 GMT
RUN cmd /S /C #(nop) COPY file:0b6475b59bf6bfe6c1030fd41ea501af74fd46ae70fd98c58683b35f8ed498ff in C:\nats-server.exe 
# Wed, 09 Sep 2020 17:12:33 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Sep 2020 17:12:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Sep 2020 17:12:34 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Sep 2020 17:12:35 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ecf9bb62dc6eedea9fd367628f8715dea75b7d2053afa4b5121e7809aa692139`  
		Size: 101.2 MB (101239122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a993e00682bb4be271d74c200e8e9d454b07999d7ab172f3b14fe72883380722`  
		Last Modified: Wed, 09 Sep 2020 17:16:30 GMT  
		Size: 929.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2582374a52a2ff5b9749c0da3753f314eebed73312c429dedd53254e3439381`  
		Last Modified: Wed, 09 Sep 2020 17:16:31 GMT  
		Size: 4.0 MB (4037991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1ddaa896f4f824bc34f5423c4a584085484ad6726210c5e85deb31b96dcecf`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 1.5 KB (1473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1c9a98b8493177510bd243f069f3169cf0575b5dbaeccaed59ec06115e30a1`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2065dc75ba87a95592c8d5d558eafa92ac761f14b53075fbf4baf04f30b1c6`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023bb1ddc2afbcca6549888de223caebd1fdb23f9744ddde1ab091e60b0c505e`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.8-nanoserver-1809`

```console
$ docker pull nats@sha256:43a61a1fde7c2a6eb37e1ca9f9fc62c070d499448ba952313e7e4455be147fbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `nats:2.1.8-nanoserver-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats@sha256:f4f74a489fc4190ec1f80cfd0c51e63462ccdbe6da88eb8e817106bb4c734469
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.3 MB (105282104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23265cf7e8f5821431c1b7add8531891db26bdc7bfd497a674244d5bfd37e21a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Sep 2020 12:08:18 GMT
RUN Apply image 1809-amd64
# Wed, 09 Sep 2020 17:12:30 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 17:12:32 GMT
RUN cmd /S /C #(nop) COPY file:0b6475b59bf6bfe6c1030fd41ea501af74fd46ae70fd98c58683b35f8ed498ff in C:\nats-server.exe 
# Wed, 09 Sep 2020 17:12:33 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Sep 2020 17:12:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Sep 2020 17:12:34 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Sep 2020 17:12:35 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ecf9bb62dc6eedea9fd367628f8715dea75b7d2053afa4b5121e7809aa692139`  
		Size: 101.2 MB (101239122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a993e00682bb4be271d74c200e8e9d454b07999d7ab172f3b14fe72883380722`  
		Last Modified: Wed, 09 Sep 2020 17:16:30 GMT  
		Size: 929.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2582374a52a2ff5b9749c0da3753f314eebed73312c429dedd53254e3439381`  
		Last Modified: Wed, 09 Sep 2020 17:16:31 GMT  
		Size: 4.0 MB (4037991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1ddaa896f4f824bc34f5423c4a584085484ad6726210c5e85deb31b96dcecf`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 1.5 KB (1473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1c9a98b8493177510bd243f069f3169cf0575b5dbaeccaed59ec06115e30a1`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2065dc75ba87a95592c8d5d558eafa92ac761f14b53075fbf4baf04f30b1c6`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023bb1ddc2afbcca6549888de223caebd1fdb23f9744ddde1ab091e60b0c505e`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 860.0 B  
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
$ docker pull nats@sha256:3023386edd4dca01ea2eb1bf9a14268388af532e86616ef4f89fbab26823b78a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64
	-	windows version 10.0.14393.3930; amd64

### `nats:2.1.8-windowsservercore` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats@sha256:1c83509a0dd49bb818407142b5595766fc8cadb59834e72c0a91deaea371ff34
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2369206825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06a6b490bf0f236facc1bf15bf5fbab8a4741401eb02c00e2bf0f129dd66c20d`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Sep 2020 13:15:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Sep 2020 17:10:34 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 17:10:34 GMT
ENV NATS_SERVER=2.1.8
# Wed, 09 Sep 2020 17:10:35 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 09 Sep 2020 17:10:35 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 09 Sep 2020 17:11:05 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Sep 2020 17:12:10 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Sep 2020 17:12:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Sep 2020 17:12:12 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Sep 2020 17:12:13 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Sep 2020 17:12:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1df31adcc7026c3bf0cb32832a3f307dd6e1e54b8b3e050f8a73b5caee674d88`  
		Last Modified: Wed, 09 Sep 2020 16:48:51 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a005485001c0802bc2ee93661375bfb4c868e16c3f5678debf00f29a8bb26386`  
		Last Modified: Wed, 09 Sep 2020 17:16:08 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662e6fbc5f9e16fc0afc4d05927cd1e64bfa92f69d228567abe407bb72908aaf`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7151925f65e3cf12e20bc6f6aa94dfb90b475195bea0a8bd3c8d70d21fe6e7`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf309bd49456f53f290cc9143ca63dc647713cb7981d22d61d7f8b18548b8ae`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fd4c97d4d46deef398e38f156ba05f404a8de7e7f7915b45a96e1b84c98e2e`  
		Last Modified: Wed, 09 Sep 2020 17:16:11 GMT  
		Size: 4.8 MB (4784097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39896e9d43e963384628807bede8a7bea2735860d8797978d74cdccb2db3cccc`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 13.1 MB (13139733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303f12072d6a77ef8f3b35b86cd6fd3a37c88fdd85e2a20d6946ad7fdb5678b4`  
		Last Modified: Wed, 09 Sep 2020 17:16:03 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02cf56909eff26727cabe26c37adb7b07aa76875550f66e267c0e9044d8f19c7`  
		Last Modified: Wed, 09 Sep 2020 17:16:03 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0c7ccbe6779b4f737d7987f4246dc066853208e9957364e0ea8e0d4ee07b47`  
		Last Modified: Wed, 09 Sep 2020 17:16:04 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a250cb3a50140ec9efe6f52457ea634df38df6babd373210cf8c5abb888f7a29`  
		Last Modified: Wed, 09 Sep 2020 17:16:03 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.8-windowsservercore` - windows version 10.0.14393.3930; amd64

```console
$ docker pull nats@sha256:281ee36c5f01f3f13192b7d9679e9ae68d89c2efb0d69f3e065fe29832ebc1a7
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5758575718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c71f48677d301c4540845a160ba3f4b3d6b2922f3032940a417555ff8ae48031`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Sep 2020 13:23:04 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Sep 2020 17:12:41 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 17:12:41 GMT
ENV NATS_SERVER=2.1.8
# Wed, 09 Sep 2020 17:12:42 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 09 Sep 2020 17:12:43 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 09 Sep 2020 17:13:51 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Sep 2020 17:15:26 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Sep 2020 17:15:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Sep 2020 17:15:28 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Sep 2020 17:15:29 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Sep 2020 17:15:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1d56eeebea105bba2dd1879a89adb012f98cf42708c0f36ca4af683db7162a2`  
		Last Modified: Wed, 09 Sep 2020 16:49:22 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4d96d0f21f7d823b426589ab2a404cd548354f8d03ceb98ed43812aa4ea498`  
		Last Modified: Wed, 09 Sep 2020 17:16:52 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9622b50495de28ed9ac7a828c8c525f5d1f3fe10f018169a78a937f320ce673`  
		Last Modified: Wed, 09 Sep 2020 17:16:49 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693bf8afbdb7ba6b5c59a194e3aefcfa41d2ad4c62e07d0961f180475570c386`  
		Last Modified: Wed, 09 Sep 2020 17:16:49 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b791adbede0214cebdc3b0f107e4d8be1105f272f85730e56a9c4bf5d44bed`  
		Last Modified: Wed, 09 Sep 2020 17:16:49 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d5083dfc8cb493d24c2ea383b470122bcff20c1348d9c40c837770030d8628`  
		Last Modified: Wed, 09 Sep 2020 17:16:50 GMT  
		Size: 5.4 MB (5379065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9444d0693ec2f93eb3184f285edbd5be7140a93d9c4309b7133979c5b5e4b34a`  
		Last Modified: Wed, 09 Sep 2020 17:17:03 GMT  
		Size: 13.9 MB (13931410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f0768454035fe701badc16b0bc29578cccb8738206c796ba98b4c1bc44718b`  
		Last Modified: Wed, 09 Sep 2020 17:16:46 GMT  
		Size: 1.7 KB (1681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de26bc51804e14983351214fb629d39bb48d1aab8771e64f000ff4bf51b2268d`  
		Last Modified: Wed, 09 Sep 2020 17:16:46 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74800b43b5c09e14a9ff54d17fac976049b117d63e9ae3e6fdd2855b6cc334c9`  
		Last Modified: Wed, 09 Sep 2020 17:16:47 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92161369e5b87a001a435fffd1802842044b222b30d4fce6964d39a2ab66d896`  
		Last Modified: Wed, 09 Sep 2020 17:16:46 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.8-windowsservercore-1809`

```console
$ docker pull nats@sha256:68052566a345b1974727afb0e13ccf5da8cd92efabede8c67f188abaabecdac9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `nats:2.1.8-windowsservercore-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats@sha256:1c83509a0dd49bb818407142b5595766fc8cadb59834e72c0a91deaea371ff34
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2369206825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06a6b490bf0f236facc1bf15bf5fbab8a4741401eb02c00e2bf0f129dd66c20d`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Sep 2020 13:15:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Sep 2020 17:10:34 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 17:10:34 GMT
ENV NATS_SERVER=2.1.8
# Wed, 09 Sep 2020 17:10:35 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 09 Sep 2020 17:10:35 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 09 Sep 2020 17:11:05 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Sep 2020 17:12:10 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Sep 2020 17:12:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Sep 2020 17:12:12 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Sep 2020 17:12:13 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Sep 2020 17:12:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1df31adcc7026c3bf0cb32832a3f307dd6e1e54b8b3e050f8a73b5caee674d88`  
		Last Modified: Wed, 09 Sep 2020 16:48:51 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a005485001c0802bc2ee93661375bfb4c868e16c3f5678debf00f29a8bb26386`  
		Last Modified: Wed, 09 Sep 2020 17:16:08 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662e6fbc5f9e16fc0afc4d05927cd1e64bfa92f69d228567abe407bb72908aaf`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7151925f65e3cf12e20bc6f6aa94dfb90b475195bea0a8bd3c8d70d21fe6e7`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf309bd49456f53f290cc9143ca63dc647713cb7981d22d61d7f8b18548b8ae`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fd4c97d4d46deef398e38f156ba05f404a8de7e7f7915b45a96e1b84c98e2e`  
		Last Modified: Wed, 09 Sep 2020 17:16:11 GMT  
		Size: 4.8 MB (4784097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39896e9d43e963384628807bede8a7bea2735860d8797978d74cdccb2db3cccc`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 13.1 MB (13139733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303f12072d6a77ef8f3b35b86cd6fd3a37c88fdd85e2a20d6946ad7fdb5678b4`  
		Last Modified: Wed, 09 Sep 2020 17:16:03 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02cf56909eff26727cabe26c37adb7b07aa76875550f66e267c0e9044d8f19c7`  
		Last Modified: Wed, 09 Sep 2020 17:16:03 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0c7ccbe6779b4f737d7987f4246dc066853208e9957364e0ea8e0d4ee07b47`  
		Last Modified: Wed, 09 Sep 2020 17:16:04 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a250cb3a50140ec9efe6f52457ea634df38df6babd373210cf8c5abb888f7a29`  
		Last Modified: Wed, 09 Sep 2020 17:16:03 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.8-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:e0113341e4407f3e09685758839e17a425ac36640e0b8ef2c1b72f61ef0f50ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3930; amd64

### `nats:2.1.8-windowsservercore-ltsc2016` - windows version 10.0.14393.3930; amd64

```console
$ docker pull nats@sha256:281ee36c5f01f3f13192b7d9679e9ae68d89c2efb0d69f3e065fe29832ebc1a7
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5758575718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c71f48677d301c4540845a160ba3f4b3d6b2922f3032940a417555ff8ae48031`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Sep 2020 13:23:04 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Sep 2020 17:12:41 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 17:12:41 GMT
ENV NATS_SERVER=2.1.8
# Wed, 09 Sep 2020 17:12:42 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 09 Sep 2020 17:12:43 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 09 Sep 2020 17:13:51 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Sep 2020 17:15:26 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Sep 2020 17:15:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Sep 2020 17:15:28 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Sep 2020 17:15:29 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Sep 2020 17:15:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1d56eeebea105bba2dd1879a89adb012f98cf42708c0f36ca4af683db7162a2`  
		Last Modified: Wed, 09 Sep 2020 16:49:22 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4d96d0f21f7d823b426589ab2a404cd548354f8d03ceb98ed43812aa4ea498`  
		Last Modified: Wed, 09 Sep 2020 17:16:52 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9622b50495de28ed9ac7a828c8c525f5d1f3fe10f018169a78a937f320ce673`  
		Last Modified: Wed, 09 Sep 2020 17:16:49 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693bf8afbdb7ba6b5c59a194e3aefcfa41d2ad4c62e07d0961f180475570c386`  
		Last Modified: Wed, 09 Sep 2020 17:16:49 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b791adbede0214cebdc3b0f107e4d8be1105f272f85730e56a9c4bf5d44bed`  
		Last Modified: Wed, 09 Sep 2020 17:16:49 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d5083dfc8cb493d24c2ea383b470122bcff20c1348d9c40c837770030d8628`  
		Last Modified: Wed, 09 Sep 2020 17:16:50 GMT  
		Size: 5.4 MB (5379065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9444d0693ec2f93eb3184f285edbd5be7140a93d9c4309b7133979c5b5e4b34a`  
		Last Modified: Wed, 09 Sep 2020 17:17:03 GMT  
		Size: 13.9 MB (13931410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f0768454035fe701badc16b0bc29578cccb8738206c796ba98b4c1bc44718b`  
		Last Modified: Wed, 09 Sep 2020 17:16:46 GMT  
		Size: 1.7 KB (1681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de26bc51804e14983351214fb629d39bb48d1aab8771e64f000ff4bf51b2268d`  
		Last Modified: Wed, 09 Sep 2020 17:16:46 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74800b43b5c09e14a9ff54d17fac976049b117d63e9ae3e6fdd2855b6cc334c9`  
		Last Modified: Wed, 09 Sep 2020 17:16:47 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92161369e5b87a001a435fffd1802842044b222b30d4fce6964d39a2ab66d896`  
		Last Modified: Wed, 09 Sep 2020 17:16:46 GMT  
		Size: 1.1 KB (1128 bytes)  
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
$ docker pull nats@sha256:43a61a1fde7c2a6eb37e1ca9f9fc62c070d499448ba952313e7e4455be147fbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `nats:2.1-nanoserver` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats@sha256:f4f74a489fc4190ec1f80cfd0c51e63462ccdbe6da88eb8e817106bb4c734469
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.3 MB (105282104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23265cf7e8f5821431c1b7add8531891db26bdc7bfd497a674244d5bfd37e21a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Sep 2020 12:08:18 GMT
RUN Apply image 1809-amd64
# Wed, 09 Sep 2020 17:12:30 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 17:12:32 GMT
RUN cmd /S /C #(nop) COPY file:0b6475b59bf6bfe6c1030fd41ea501af74fd46ae70fd98c58683b35f8ed498ff in C:\nats-server.exe 
# Wed, 09 Sep 2020 17:12:33 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Sep 2020 17:12:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Sep 2020 17:12:34 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Sep 2020 17:12:35 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ecf9bb62dc6eedea9fd367628f8715dea75b7d2053afa4b5121e7809aa692139`  
		Size: 101.2 MB (101239122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a993e00682bb4be271d74c200e8e9d454b07999d7ab172f3b14fe72883380722`  
		Last Modified: Wed, 09 Sep 2020 17:16:30 GMT  
		Size: 929.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2582374a52a2ff5b9749c0da3753f314eebed73312c429dedd53254e3439381`  
		Last Modified: Wed, 09 Sep 2020 17:16:31 GMT  
		Size: 4.0 MB (4037991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1ddaa896f4f824bc34f5423c4a584085484ad6726210c5e85deb31b96dcecf`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 1.5 KB (1473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1c9a98b8493177510bd243f069f3169cf0575b5dbaeccaed59ec06115e30a1`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2065dc75ba87a95592c8d5d558eafa92ac761f14b53075fbf4baf04f30b1c6`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023bb1ddc2afbcca6549888de223caebd1fdb23f9744ddde1ab091e60b0c505e`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-nanoserver-1809`

```console
$ docker pull nats@sha256:43a61a1fde7c2a6eb37e1ca9f9fc62c070d499448ba952313e7e4455be147fbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `nats:2.1-nanoserver-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats@sha256:f4f74a489fc4190ec1f80cfd0c51e63462ccdbe6da88eb8e817106bb4c734469
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.3 MB (105282104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23265cf7e8f5821431c1b7add8531891db26bdc7bfd497a674244d5bfd37e21a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Sep 2020 12:08:18 GMT
RUN Apply image 1809-amd64
# Wed, 09 Sep 2020 17:12:30 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 17:12:32 GMT
RUN cmd /S /C #(nop) COPY file:0b6475b59bf6bfe6c1030fd41ea501af74fd46ae70fd98c58683b35f8ed498ff in C:\nats-server.exe 
# Wed, 09 Sep 2020 17:12:33 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Sep 2020 17:12:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Sep 2020 17:12:34 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Sep 2020 17:12:35 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ecf9bb62dc6eedea9fd367628f8715dea75b7d2053afa4b5121e7809aa692139`  
		Size: 101.2 MB (101239122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a993e00682bb4be271d74c200e8e9d454b07999d7ab172f3b14fe72883380722`  
		Last Modified: Wed, 09 Sep 2020 17:16:30 GMT  
		Size: 929.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2582374a52a2ff5b9749c0da3753f314eebed73312c429dedd53254e3439381`  
		Last Modified: Wed, 09 Sep 2020 17:16:31 GMT  
		Size: 4.0 MB (4037991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1ddaa896f4f824bc34f5423c4a584085484ad6726210c5e85deb31b96dcecf`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 1.5 KB (1473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1c9a98b8493177510bd243f069f3169cf0575b5dbaeccaed59ec06115e30a1`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2065dc75ba87a95592c8d5d558eafa92ac761f14b53075fbf4baf04f30b1c6`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023bb1ddc2afbcca6549888de223caebd1fdb23f9744ddde1ab091e60b0c505e`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 860.0 B  
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
$ docker pull nats@sha256:3023386edd4dca01ea2eb1bf9a14268388af532e86616ef4f89fbab26823b78a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64
	-	windows version 10.0.14393.3930; amd64

### `nats:2.1-windowsservercore` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats@sha256:1c83509a0dd49bb818407142b5595766fc8cadb59834e72c0a91deaea371ff34
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2369206825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06a6b490bf0f236facc1bf15bf5fbab8a4741401eb02c00e2bf0f129dd66c20d`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Sep 2020 13:15:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Sep 2020 17:10:34 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 17:10:34 GMT
ENV NATS_SERVER=2.1.8
# Wed, 09 Sep 2020 17:10:35 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 09 Sep 2020 17:10:35 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 09 Sep 2020 17:11:05 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Sep 2020 17:12:10 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Sep 2020 17:12:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Sep 2020 17:12:12 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Sep 2020 17:12:13 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Sep 2020 17:12:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1df31adcc7026c3bf0cb32832a3f307dd6e1e54b8b3e050f8a73b5caee674d88`  
		Last Modified: Wed, 09 Sep 2020 16:48:51 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a005485001c0802bc2ee93661375bfb4c868e16c3f5678debf00f29a8bb26386`  
		Last Modified: Wed, 09 Sep 2020 17:16:08 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662e6fbc5f9e16fc0afc4d05927cd1e64bfa92f69d228567abe407bb72908aaf`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7151925f65e3cf12e20bc6f6aa94dfb90b475195bea0a8bd3c8d70d21fe6e7`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf309bd49456f53f290cc9143ca63dc647713cb7981d22d61d7f8b18548b8ae`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fd4c97d4d46deef398e38f156ba05f404a8de7e7f7915b45a96e1b84c98e2e`  
		Last Modified: Wed, 09 Sep 2020 17:16:11 GMT  
		Size: 4.8 MB (4784097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39896e9d43e963384628807bede8a7bea2735860d8797978d74cdccb2db3cccc`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 13.1 MB (13139733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303f12072d6a77ef8f3b35b86cd6fd3a37c88fdd85e2a20d6946ad7fdb5678b4`  
		Last Modified: Wed, 09 Sep 2020 17:16:03 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02cf56909eff26727cabe26c37adb7b07aa76875550f66e267c0e9044d8f19c7`  
		Last Modified: Wed, 09 Sep 2020 17:16:03 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0c7ccbe6779b4f737d7987f4246dc066853208e9957364e0ea8e0d4ee07b47`  
		Last Modified: Wed, 09 Sep 2020 17:16:04 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a250cb3a50140ec9efe6f52457ea634df38df6babd373210cf8c5abb888f7a29`  
		Last Modified: Wed, 09 Sep 2020 17:16:03 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-windowsservercore` - windows version 10.0.14393.3930; amd64

```console
$ docker pull nats@sha256:281ee36c5f01f3f13192b7d9679e9ae68d89c2efb0d69f3e065fe29832ebc1a7
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5758575718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c71f48677d301c4540845a160ba3f4b3d6b2922f3032940a417555ff8ae48031`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Sep 2020 13:23:04 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Sep 2020 17:12:41 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 17:12:41 GMT
ENV NATS_SERVER=2.1.8
# Wed, 09 Sep 2020 17:12:42 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 09 Sep 2020 17:12:43 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 09 Sep 2020 17:13:51 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Sep 2020 17:15:26 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Sep 2020 17:15:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Sep 2020 17:15:28 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Sep 2020 17:15:29 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Sep 2020 17:15:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1d56eeebea105bba2dd1879a89adb012f98cf42708c0f36ca4af683db7162a2`  
		Last Modified: Wed, 09 Sep 2020 16:49:22 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4d96d0f21f7d823b426589ab2a404cd548354f8d03ceb98ed43812aa4ea498`  
		Last Modified: Wed, 09 Sep 2020 17:16:52 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9622b50495de28ed9ac7a828c8c525f5d1f3fe10f018169a78a937f320ce673`  
		Last Modified: Wed, 09 Sep 2020 17:16:49 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693bf8afbdb7ba6b5c59a194e3aefcfa41d2ad4c62e07d0961f180475570c386`  
		Last Modified: Wed, 09 Sep 2020 17:16:49 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b791adbede0214cebdc3b0f107e4d8be1105f272f85730e56a9c4bf5d44bed`  
		Last Modified: Wed, 09 Sep 2020 17:16:49 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d5083dfc8cb493d24c2ea383b470122bcff20c1348d9c40c837770030d8628`  
		Last Modified: Wed, 09 Sep 2020 17:16:50 GMT  
		Size: 5.4 MB (5379065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9444d0693ec2f93eb3184f285edbd5be7140a93d9c4309b7133979c5b5e4b34a`  
		Last Modified: Wed, 09 Sep 2020 17:17:03 GMT  
		Size: 13.9 MB (13931410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f0768454035fe701badc16b0bc29578cccb8738206c796ba98b4c1bc44718b`  
		Last Modified: Wed, 09 Sep 2020 17:16:46 GMT  
		Size: 1.7 KB (1681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de26bc51804e14983351214fb629d39bb48d1aab8771e64f000ff4bf51b2268d`  
		Last Modified: Wed, 09 Sep 2020 17:16:46 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74800b43b5c09e14a9ff54d17fac976049b117d63e9ae3e6fdd2855b6cc334c9`  
		Last Modified: Wed, 09 Sep 2020 17:16:47 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92161369e5b87a001a435fffd1802842044b222b30d4fce6964d39a2ab66d896`  
		Last Modified: Wed, 09 Sep 2020 17:16:46 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-windowsservercore-1809`

```console
$ docker pull nats@sha256:68052566a345b1974727afb0e13ccf5da8cd92efabede8c67f188abaabecdac9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `nats:2.1-windowsservercore-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats@sha256:1c83509a0dd49bb818407142b5595766fc8cadb59834e72c0a91deaea371ff34
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2369206825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06a6b490bf0f236facc1bf15bf5fbab8a4741401eb02c00e2bf0f129dd66c20d`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Sep 2020 13:15:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Sep 2020 17:10:34 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 17:10:34 GMT
ENV NATS_SERVER=2.1.8
# Wed, 09 Sep 2020 17:10:35 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 09 Sep 2020 17:10:35 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 09 Sep 2020 17:11:05 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Sep 2020 17:12:10 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Sep 2020 17:12:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Sep 2020 17:12:12 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Sep 2020 17:12:13 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Sep 2020 17:12:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1df31adcc7026c3bf0cb32832a3f307dd6e1e54b8b3e050f8a73b5caee674d88`  
		Last Modified: Wed, 09 Sep 2020 16:48:51 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a005485001c0802bc2ee93661375bfb4c868e16c3f5678debf00f29a8bb26386`  
		Last Modified: Wed, 09 Sep 2020 17:16:08 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662e6fbc5f9e16fc0afc4d05927cd1e64bfa92f69d228567abe407bb72908aaf`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7151925f65e3cf12e20bc6f6aa94dfb90b475195bea0a8bd3c8d70d21fe6e7`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf309bd49456f53f290cc9143ca63dc647713cb7981d22d61d7f8b18548b8ae`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fd4c97d4d46deef398e38f156ba05f404a8de7e7f7915b45a96e1b84c98e2e`  
		Last Modified: Wed, 09 Sep 2020 17:16:11 GMT  
		Size: 4.8 MB (4784097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39896e9d43e963384628807bede8a7bea2735860d8797978d74cdccb2db3cccc`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 13.1 MB (13139733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303f12072d6a77ef8f3b35b86cd6fd3a37c88fdd85e2a20d6946ad7fdb5678b4`  
		Last Modified: Wed, 09 Sep 2020 17:16:03 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02cf56909eff26727cabe26c37adb7b07aa76875550f66e267c0e9044d8f19c7`  
		Last Modified: Wed, 09 Sep 2020 17:16:03 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0c7ccbe6779b4f737d7987f4246dc066853208e9957364e0ea8e0d4ee07b47`  
		Last Modified: Wed, 09 Sep 2020 17:16:04 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a250cb3a50140ec9efe6f52457ea634df38df6babd373210cf8c5abb888f7a29`  
		Last Modified: Wed, 09 Sep 2020 17:16:03 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:e0113341e4407f3e09685758839e17a425ac36640e0b8ef2c1b72f61ef0f50ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3930; amd64

### `nats:2.1-windowsservercore-ltsc2016` - windows version 10.0.14393.3930; amd64

```console
$ docker pull nats@sha256:281ee36c5f01f3f13192b7d9679e9ae68d89c2efb0d69f3e065fe29832ebc1a7
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5758575718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c71f48677d301c4540845a160ba3f4b3d6b2922f3032940a417555ff8ae48031`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Sep 2020 13:23:04 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Sep 2020 17:12:41 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 17:12:41 GMT
ENV NATS_SERVER=2.1.8
# Wed, 09 Sep 2020 17:12:42 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 09 Sep 2020 17:12:43 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 09 Sep 2020 17:13:51 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Sep 2020 17:15:26 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Sep 2020 17:15:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Sep 2020 17:15:28 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Sep 2020 17:15:29 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Sep 2020 17:15:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1d56eeebea105bba2dd1879a89adb012f98cf42708c0f36ca4af683db7162a2`  
		Last Modified: Wed, 09 Sep 2020 16:49:22 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4d96d0f21f7d823b426589ab2a404cd548354f8d03ceb98ed43812aa4ea498`  
		Last Modified: Wed, 09 Sep 2020 17:16:52 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9622b50495de28ed9ac7a828c8c525f5d1f3fe10f018169a78a937f320ce673`  
		Last Modified: Wed, 09 Sep 2020 17:16:49 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693bf8afbdb7ba6b5c59a194e3aefcfa41d2ad4c62e07d0961f180475570c386`  
		Last Modified: Wed, 09 Sep 2020 17:16:49 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b791adbede0214cebdc3b0f107e4d8be1105f272f85730e56a9c4bf5d44bed`  
		Last Modified: Wed, 09 Sep 2020 17:16:49 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d5083dfc8cb493d24c2ea383b470122bcff20c1348d9c40c837770030d8628`  
		Last Modified: Wed, 09 Sep 2020 17:16:50 GMT  
		Size: 5.4 MB (5379065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9444d0693ec2f93eb3184f285edbd5be7140a93d9c4309b7133979c5b5e4b34a`  
		Last Modified: Wed, 09 Sep 2020 17:17:03 GMT  
		Size: 13.9 MB (13931410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f0768454035fe701badc16b0bc29578cccb8738206c796ba98b4c1bc44718b`  
		Last Modified: Wed, 09 Sep 2020 17:16:46 GMT  
		Size: 1.7 KB (1681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de26bc51804e14983351214fb629d39bb48d1aab8771e64f000ff4bf51b2268d`  
		Last Modified: Wed, 09 Sep 2020 17:16:46 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74800b43b5c09e14a9ff54d17fac976049b117d63e9ae3e6fdd2855b6cc334c9`  
		Last Modified: Wed, 09 Sep 2020 17:16:47 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92161369e5b87a001a435fffd1802842044b222b30d4fce6964d39a2ab66d896`  
		Last Modified: Wed, 09 Sep 2020 17:16:46 GMT  
		Size: 1.1 KB (1128 bytes)  
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
$ docker pull nats@sha256:43a61a1fde7c2a6eb37e1ca9f9fc62c070d499448ba952313e7e4455be147fbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats@sha256:f4f74a489fc4190ec1f80cfd0c51e63462ccdbe6da88eb8e817106bb4c734469
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.3 MB (105282104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23265cf7e8f5821431c1b7add8531891db26bdc7bfd497a674244d5bfd37e21a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Sep 2020 12:08:18 GMT
RUN Apply image 1809-amd64
# Wed, 09 Sep 2020 17:12:30 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 17:12:32 GMT
RUN cmd /S /C #(nop) COPY file:0b6475b59bf6bfe6c1030fd41ea501af74fd46ae70fd98c58683b35f8ed498ff in C:\nats-server.exe 
# Wed, 09 Sep 2020 17:12:33 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Sep 2020 17:12:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Sep 2020 17:12:34 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Sep 2020 17:12:35 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ecf9bb62dc6eedea9fd367628f8715dea75b7d2053afa4b5121e7809aa692139`  
		Size: 101.2 MB (101239122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a993e00682bb4be271d74c200e8e9d454b07999d7ab172f3b14fe72883380722`  
		Last Modified: Wed, 09 Sep 2020 17:16:30 GMT  
		Size: 929.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2582374a52a2ff5b9749c0da3753f314eebed73312c429dedd53254e3439381`  
		Last Modified: Wed, 09 Sep 2020 17:16:31 GMT  
		Size: 4.0 MB (4037991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1ddaa896f4f824bc34f5423c4a584085484ad6726210c5e85deb31b96dcecf`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 1.5 KB (1473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1c9a98b8493177510bd243f069f3169cf0575b5dbaeccaed59ec06115e30a1`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2065dc75ba87a95592c8d5d558eafa92ac761f14b53075fbf4baf04f30b1c6`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023bb1ddc2afbcca6549888de223caebd1fdb23f9744ddde1ab091e60b0c505e`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:43a61a1fde7c2a6eb37e1ca9f9fc62c070d499448ba952313e7e4455be147fbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats@sha256:f4f74a489fc4190ec1f80cfd0c51e63462ccdbe6da88eb8e817106bb4c734469
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.3 MB (105282104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23265cf7e8f5821431c1b7add8531891db26bdc7bfd497a674244d5bfd37e21a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Sep 2020 12:08:18 GMT
RUN Apply image 1809-amd64
# Wed, 09 Sep 2020 17:12:30 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 17:12:32 GMT
RUN cmd /S /C #(nop) COPY file:0b6475b59bf6bfe6c1030fd41ea501af74fd46ae70fd98c58683b35f8ed498ff in C:\nats-server.exe 
# Wed, 09 Sep 2020 17:12:33 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Sep 2020 17:12:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Sep 2020 17:12:34 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Sep 2020 17:12:35 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ecf9bb62dc6eedea9fd367628f8715dea75b7d2053afa4b5121e7809aa692139`  
		Size: 101.2 MB (101239122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a993e00682bb4be271d74c200e8e9d454b07999d7ab172f3b14fe72883380722`  
		Last Modified: Wed, 09 Sep 2020 17:16:30 GMT  
		Size: 929.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2582374a52a2ff5b9749c0da3753f314eebed73312c429dedd53254e3439381`  
		Last Modified: Wed, 09 Sep 2020 17:16:31 GMT  
		Size: 4.0 MB (4037991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1ddaa896f4f824bc34f5423c4a584085484ad6726210c5e85deb31b96dcecf`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 1.5 KB (1473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1c9a98b8493177510bd243f069f3169cf0575b5dbaeccaed59ec06115e30a1`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2065dc75ba87a95592c8d5d558eafa92ac761f14b53075fbf4baf04f30b1c6`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023bb1ddc2afbcca6549888de223caebd1fdb23f9744ddde1ab091e60b0c505e`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 860.0 B  
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
$ docker pull nats@sha256:3023386edd4dca01ea2eb1bf9a14268388af532e86616ef4f89fbab26823b78a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64
	-	windows version 10.0.14393.3930; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats@sha256:1c83509a0dd49bb818407142b5595766fc8cadb59834e72c0a91deaea371ff34
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2369206825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06a6b490bf0f236facc1bf15bf5fbab8a4741401eb02c00e2bf0f129dd66c20d`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Sep 2020 13:15:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Sep 2020 17:10:34 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 17:10:34 GMT
ENV NATS_SERVER=2.1.8
# Wed, 09 Sep 2020 17:10:35 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 09 Sep 2020 17:10:35 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 09 Sep 2020 17:11:05 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Sep 2020 17:12:10 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Sep 2020 17:12:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Sep 2020 17:12:12 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Sep 2020 17:12:13 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Sep 2020 17:12:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1df31adcc7026c3bf0cb32832a3f307dd6e1e54b8b3e050f8a73b5caee674d88`  
		Last Modified: Wed, 09 Sep 2020 16:48:51 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a005485001c0802bc2ee93661375bfb4c868e16c3f5678debf00f29a8bb26386`  
		Last Modified: Wed, 09 Sep 2020 17:16:08 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662e6fbc5f9e16fc0afc4d05927cd1e64bfa92f69d228567abe407bb72908aaf`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7151925f65e3cf12e20bc6f6aa94dfb90b475195bea0a8bd3c8d70d21fe6e7`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf309bd49456f53f290cc9143ca63dc647713cb7981d22d61d7f8b18548b8ae`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fd4c97d4d46deef398e38f156ba05f404a8de7e7f7915b45a96e1b84c98e2e`  
		Last Modified: Wed, 09 Sep 2020 17:16:11 GMT  
		Size: 4.8 MB (4784097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39896e9d43e963384628807bede8a7bea2735860d8797978d74cdccb2db3cccc`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 13.1 MB (13139733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303f12072d6a77ef8f3b35b86cd6fd3a37c88fdd85e2a20d6946ad7fdb5678b4`  
		Last Modified: Wed, 09 Sep 2020 17:16:03 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02cf56909eff26727cabe26c37adb7b07aa76875550f66e267c0e9044d8f19c7`  
		Last Modified: Wed, 09 Sep 2020 17:16:03 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0c7ccbe6779b4f737d7987f4246dc066853208e9957364e0ea8e0d4ee07b47`  
		Last Modified: Wed, 09 Sep 2020 17:16:04 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a250cb3a50140ec9efe6f52457ea634df38df6babd373210cf8c5abb888f7a29`  
		Last Modified: Wed, 09 Sep 2020 17:16:03 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.3930; amd64

```console
$ docker pull nats@sha256:281ee36c5f01f3f13192b7d9679e9ae68d89c2efb0d69f3e065fe29832ebc1a7
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5758575718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c71f48677d301c4540845a160ba3f4b3d6b2922f3032940a417555ff8ae48031`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Sep 2020 13:23:04 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Sep 2020 17:12:41 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 17:12:41 GMT
ENV NATS_SERVER=2.1.8
# Wed, 09 Sep 2020 17:12:42 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 09 Sep 2020 17:12:43 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 09 Sep 2020 17:13:51 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Sep 2020 17:15:26 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Sep 2020 17:15:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Sep 2020 17:15:28 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Sep 2020 17:15:29 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Sep 2020 17:15:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1d56eeebea105bba2dd1879a89adb012f98cf42708c0f36ca4af683db7162a2`  
		Last Modified: Wed, 09 Sep 2020 16:49:22 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4d96d0f21f7d823b426589ab2a404cd548354f8d03ceb98ed43812aa4ea498`  
		Last Modified: Wed, 09 Sep 2020 17:16:52 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9622b50495de28ed9ac7a828c8c525f5d1f3fe10f018169a78a937f320ce673`  
		Last Modified: Wed, 09 Sep 2020 17:16:49 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693bf8afbdb7ba6b5c59a194e3aefcfa41d2ad4c62e07d0961f180475570c386`  
		Last Modified: Wed, 09 Sep 2020 17:16:49 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b791adbede0214cebdc3b0f107e4d8be1105f272f85730e56a9c4bf5d44bed`  
		Last Modified: Wed, 09 Sep 2020 17:16:49 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d5083dfc8cb493d24c2ea383b470122bcff20c1348d9c40c837770030d8628`  
		Last Modified: Wed, 09 Sep 2020 17:16:50 GMT  
		Size: 5.4 MB (5379065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9444d0693ec2f93eb3184f285edbd5be7140a93d9c4309b7133979c5b5e4b34a`  
		Last Modified: Wed, 09 Sep 2020 17:17:03 GMT  
		Size: 13.9 MB (13931410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f0768454035fe701badc16b0bc29578cccb8738206c796ba98b4c1bc44718b`  
		Last Modified: Wed, 09 Sep 2020 17:16:46 GMT  
		Size: 1.7 KB (1681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de26bc51804e14983351214fb629d39bb48d1aab8771e64f000ff4bf51b2268d`  
		Last Modified: Wed, 09 Sep 2020 17:16:46 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74800b43b5c09e14a9ff54d17fac976049b117d63e9ae3e6fdd2855b6cc334c9`  
		Last Modified: Wed, 09 Sep 2020 17:16:47 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92161369e5b87a001a435fffd1802842044b222b30d4fce6964d39a2ab66d896`  
		Last Modified: Wed, 09 Sep 2020 17:16:46 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:68052566a345b1974727afb0e13ccf5da8cd92efabede8c67f188abaabecdac9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats@sha256:1c83509a0dd49bb818407142b5595766fc8cadb59834e72c0a91deaea371ff34
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2369206825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06a6b490bf0f236facc1bf15bf5fbab8a4741401eb02c00e2bf0f129dd66c20d`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Sep 2020 13:15:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Sep 2020 17:10:34 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 17:10:34 GMT
ENV NATS_SERVER=2.1.8
# Wed, 09 Sep 2020 17:10:35 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 09 Sep 2020 17:10:35 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 09 Sep 2020 17:11:05 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Sep 2020 17:12:10 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Sep 2020 17:12:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Sep 2020 17:12:12 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Sep 2020 17:12:13 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Sep 2020 17:12:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1df31adcc7026c3bf0cb32832a3f307dd6e1e54b8b3e050f8a73b5caee674d88`  
		Last Modified: Wed, 09 Sep 2020 16:48:51 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a005485001c0802bc2ee93661375bfb4c868e16c3f5678debf00f29a8bb26386`  
		Last Modified: Wed, 09 Sep 2020 17:16:08 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662e6fbc5f9e16fc0afc4d05927cd1e64bfa92f69d228567abe407bb72908aaf`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7151925f65e3cf12e20bc6f6aa94dfb90b475195bea0a8bd3c8d70d21fe6e7`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf309bd49456f53f290cc9143ca63dc647713cb7981d22d61d7f8b18548b8ae`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fd4c97d4d46deef398e38f156ba05f404a8de7e7f7915b45a96e1b84c98e2e`  
		Last Modified: Wed, 09 Sep 2020 17:16:11 GMT  
		Size: 4.8 MB (4784097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39896e9d43e963384628807bede8a7bea2735860d8797978d74cdccb2db3cccc`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 13.1 MB (13139733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303f12072d6a77ef8f3b35b86cd6fd3a37c88fdd85e2a20d6946ad7fdb5678b4`  
		Last Modified: Wed, 09 Sep 2020 17:16:03 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02cf56909eff26727cabe26c37adb7b07aa76875550f66e267c0e9044d8f19c7`  
		Last Modified: Wed, 09 Sep 2020 17:16:03 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0c7ccbe6779b4f737d7987f4246dc066853208e9957364e0ea8e0d4ee07b47`  
		Last Modified: Wed, 09 Sep 2020 17:16:04 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a250cb3a50140ec9efe6f52457ea634df38df6babd373210cf8c5abb888f7a29`  
		Last Modified: Wed, 09 Sep 2020 17:16:03 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:e0113341e4407f3e09685758839e17a425ac36640e0b8ef2c1b72f61ef0f50ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3930; amd64

### `nats:2-windowsservercore-ltsc2016` - windows version 10.0.14393.3930; amd64

```console
$ docker pull nats@sha256:281ee36c5f01f3f13192b7d9679e9ae68d89c2efb0d69f3e065fe29832ebc1a7
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5758575718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c71f48677d301c4540845a160ba3f4b3d6b2922f3032940a417555ff8ae48031`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Sep 2020 13:23:04 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Sep 2020 17:12:41 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 17:12:41 GMT
ENV NATS_SERVER=2.1.8
# Wed, 09 Sep 2020 17:12:42 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 09 Sep 2020 17:12:43 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 09 Sep 2020 17:13:51 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Sep 2020 17:15:26 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Sep 2020 17:15:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Sep 2020 17:15:28 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Sep 2020 17:15:29 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Sep 2020 17:15:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1d56eeebea105bba2dd1879a89adb012f98cf42708c0f36ca4af683db7162a2`  
		Last Modified: Wed, 09 Sep 2020 16:49:22 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4d96d0f21f7d823b426589ab2a404cd548354f8d03ceb98ed43812aa4ea498`  
		Last Modified: Wed, 09 Sep 2020 17:16:52 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9622b50495de28ed9ac7a828c8c525f5d1f3fe10f018169a78a937f320ce673`  
		Last Modified: Wed, 09 Sep 2020 17:16:49 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693bf8afbdb7ba6b5c59a194e3aefcfa41d2ad4c62e07d0961f180475570c386`  
		Last Modified: Wed, 09 Sep 2020 17:16:49 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b791adbede0214cebdc3b0f107e4d8be1105f272f85730e56a9c4bf5d44bed`  
		Last Modified: Wed, 09 Sep 2020 17:16:49 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d5083dfc8cb493d24c2ea383b470122bcff20c1348d9c40c837770030d8628`  
		Last Modified: Wed, 09 Sep 2020 17:16:50 GMT  
		Size: 5.4 MB (5379065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9444d0693ec2f93eb3184f285edbd5be7140a93d9c4309b7133979c5b5e4b34a`  
		Last Modified: Wed, 09 Sep 2020 17:17:03 GMT  
		Size: 13.9 MB (13931410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f0768454035fe701badc16b0bc29578cccb8738206c796ba98b4c1bc44718b`  
		Last Modified: Wed, 09 Sep 2020 17:16:46 GMT  
		Size: 1.7 KB (1681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de26bc51804e14983351214fb629d39bb48d1aab8771e64f000ff4bf51b2268d`  
		Last Modified: Wed, 09 Sep 2020 17:16:46 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74800b43b5c09e14a9ff54d17fac976049b117d63e9ae3e6fdd2855b6cc334c9`  
		Last Modified: Wed, 09 Sep 2020 17:16:47 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92161369e5b87a001a435fffd1802842044b222b30d4fce6964d39a2ab66d896`  
		Last Modified: Wed, 09 Sep 2020 17:16:46 GMT  
		Size: 1.1 KB (1128 bytes)  
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
$ docker pull nats@sha256:8ef9f9514ee044da7c405a5e2520771f0d1f5ad741246bb0f82a329278e0cb77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1457; amd64

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

### `nats:latest` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats@sha256:f4f74a489fc4190ec1f80cfd0c51e63462ccdbe6da88eb8e817106bb4c734469
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.3 MB (105282104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23265cf7e8f5821431c1b7add8531891db26bdc7bfd497a674244d5bfd37e21a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Sep 2020 12:08:18 GMT
RUN Apply image 1809-amd64
# Wed, 09 Sep 2020 17:12:30 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 17:12:32 GMT
RUN cmd /S /C #(nop) COPY file:0b6475b59bf6bfe6c1030fd41ea501af74fd46ae70fd98c58683b35f8ed498ff in C:\nats-server.exe 
# Wed, 09 Sep 2020 17:12:33 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Sep 2020 17:12:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Sep 2020 17:12:34 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Sep 2020 17:12:35 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ecf9bb62dc6eedea9fd367628f8715dea75b7d2053afa4b5121e7809aa692139`  
		Size: 101.2 MB (101239122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a993e00682bb4be271d74c200e8e9d454b07999d7ab172f3b14fe72883380722`  
		Last Modified: Wed, 09 Sep 2020 17:16:30 GMT  
		Size: 929.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2582374a52a2ff5b9749c0da3753f314eebed73312c429dedd53254e3439381`  
		Last Modified: Wed, 09 Sep 2020 17:16:31 GMT  
		Size: 4.0 MB (4037991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1ddaa896f4f824bc34f5423c4a584085484ad6726210c5e85deb31b96dcecf`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 1.5 KB (1473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1c9a98b8493177510bd243f069f3169cf0575b5dbaeccaed59ec06115e30a1`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2065dc75ba87a95592c8d5d558eafa92ac761f14b53075fbf4baf04f30b1c6`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023bb1ddc2afbcca6549888de223caebd1fdb23f9744ddde1ab091e60b0c505e`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 860.0 B  
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
$ docker pull nats@sha256:43a61a1fde7c2a6eb37e1ca9f9fc62c070d499448ba952313e7e4455be147fbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `nats:nanoserver` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats@sha256:f4f74a489fc4190ec1f80cfd0c51e63462ccdbe6da88eb8e817106bb4c734469
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.3 MB (105282104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23265cf7e8f5821431c1b7add8531891db26bdc7bfd497a674244d5bfd37e21a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Sep 2020 12:08:18 GMT
RUN Apply image 1809-amd64
# Wed, 09 Sep 2020 17:12:30 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 17:12:32 GMT
RUN cmd /S /C #(nop) COPY file:0b6475b59bf6bfe6c1030fd41ea501af74fd46ae70fd98c58683b35f8ed498ff in C:\nats-server.exe 
# Wed, 09 Sep 2020 17:12:33 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Sep 2020 17:12:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Sep 2020 17:12:34 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Sep 2020 17:12:35 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ecf9bb62dc6eedea9fd367628f8715dea75b7d2053afa4b5121e7809aa692139`  
		Size: 101.2 MB (101239122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a993e00682bb4be271d74c200e8e9d454b07999d7ab172f3b14fe72883380722`  
		Last Modified: Wed, 09 Sep 2020 17:16:30 GMT  
		Size: 929.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2582374a52a2ff5b9749c0da3753f314eebed73312c429dedd53254e3439381`  
		Last Modified: Wed, 09 Sep 2020 17:16:31 GMT  
		Size: 4.0 MB (4037991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1ddaa896f4f824bc34f5423c4a584085484ad6726210c5e85deb31b96dcecf`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 1.5 KB (1473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1c9a98b8493177510bd243f069f3169cf0575b5dbaeccaed59ec06115e30a1`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2065dc75ba87a95592c8d5d558eafa92ac761f14b53075fbf4baf04f30b1c6`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023bb1ddc2afbcca6549888de223caebd1fdb23f9744ddde1ab091e60b0c505e`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:43a61a1fde7c2a6eb37e1ca9f9fc62c070d499448ba952313e7e4455be147fbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats@sha256:f4f74a489fc4190ec1f80cfd0c51e63462ccdbe6da88eb8e817106bb4c734469
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.3 MB (105282104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23265cf7e8f5821431c1b7add8531891db26bdc7bfd497a674244d5bfd37e21a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Sep 2020 12:08:18 GMT
RUN Apply image 1809-amd64
# Wed, 09 Sep 2020 17:12:30 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 17:12:32 GMT
RUN cmd /S /C #(nop) COPY file:0b6475b59bf6bfe6c1030fd41ea501af74fd46ae70fd98c58683b35f8ed498ff in C:\nats-server.exe 
# Wed, 09 Sep 2020 17:12:33 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Sep 2020 17:12:34 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Sep 2020 17:12:34 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Sep 2020 17:12:35 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ecf9bb62dc6eedea9fd367628f8715dea75b7d2053afa4b5121e7809aa692139`  
		Size: 101.2 MB (101239122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a993e00682bb4be271d74c200e8e9d454b07999d7ab172f3b14fe72883380722`  
		Last Modified: Wed, 09 Sep 2020 17:16:30 GMT  
		Size: 929.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2582374a52a2ff5b9749c0da3753f314eebed73312c429dedd53254e3439381`  
		Last Modified: Wed, 09 Sep 2020 17:16:31 GMT  
		Size: 4.0 MB (4037991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1ddaa896f4f824bc34f5423c4a584085484ad6726210c5e85deb31b96dcecf`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 1.5 KB (1473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1c9a98b8493177510bd243f069f3169cf0575b5dbaeccaed59ec06115e30a1`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2065dc75ba87a95592c8d5d558eafa92ac761f14b53075fbf4baf04f30b1c6`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023bb1ddc2afbcca6549888de223caebd1fdb23f9744ddde1ab091e60b0c505e`  
		Last Modified: Wed, 09 Sep 2020 17:16:27 GMT  
		Size: 860.0 B  
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
$ docker pull nats@sha256:3023386edd4dca01ea2eb1bf9a14268388af532e86616ef4f89fbab26823b78a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64
	-	windows version 10.0.14393.3930; amd64

### `nats:windowsservercore` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats@sha256:1c83509a0dd49bb818407142b5595766fc8cadb59834e72c0a91deaea371ff34
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2369206825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06a6b490bf0f236facc1bf15bf5fbab8a4741401eb02c00e2bf0f129dd66c20d`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Sep 2020 13:15:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Sep 2020 17:10:34 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 17:10:34 GMT
ENV NATS_SERVER=2.1.8
# Wed, 09 Sep 2020 17:10:35 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 09 Sep 2020 17:10:35 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 09 Sep 2020 17:11:05 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Sep 2020 17:12:10 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Sep 2020 17:12:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Sep 2020 17:12:12 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Sep 2020 17:12:13 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Sep 2020 17:12:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1df31adcc7026c3bf0cb32832a3f307dd6e1e54b8b3e050f8a73b5caee674d88`  
		Last Modified: Wed, 09 Sep 2020 16:48:51 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a005485001c0802bc2ee93661375bfb4c868e16c3f5678debf00f29a8bb26386`  
		Last Modified: Wed, 09 Sep 2020 17:16:08 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662e6fbc5f9e16fc0afc4d05927cd1e64bfa92f69d228567abe407bb72908aaf`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7151925f65e3cf12e20bc6f6aa94dfb90b475195bea0a8bd3c8d70d21fe6e7`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf309bd49456f53f290cc9143ca63dc647713cb7981d22d61d7f8b18548b8ae`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fd4c97d4d46deef398e38f156ba05f404a8de7e7f7915b45a96e1b84c98e2e`  
		Last Modified: Wed, 09 Sep 2020 17:16:11 GMT  
		Size: 4.8 MB (4784097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39896e9d43e963384628807bede8a7bea2735860d8797978d74cdccb2db3cccc`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 13.1 MB (13139733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303f12072d6a77ef8f3b35b86cd6fd3a37c88fdd85e2a20d6946ad7fdb5678b4`  
		Last Modified: Wed, 09 Sep 2020 17:16:03 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02cf56909eff26727cabe26c37adb7b07aa76875550f66e267c0e9044d8f19c7`  
		Last Modified: Wed, 09 Sep 2020 17:16:03 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0c7ccbe6779b4f737d7987f4246dc066853208e9957364e0ea8e0d4ee07b47`  
		Last Modified: Wed, 09 Sep 2020 17:16:04 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a250cb3a50140ec9efe6f52457ea634df38df6babd373210cf8c5abb888f7a29`  
		Last Modified: Wed, 09 Sep 2020 17:16:03 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:windowsservercore` - windows version 10.0.14393.3930; amd64

```console
$ docker pull nats@sha256:281ee36c5f01f3f13192b7d9679e9ae68d89c2efb0d69f3e065fe29832ebc1a7
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5758575718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c71f48677d301c4540845a160ba3f4b3d6b2922f3032940a417555ff8ae48031`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Sep 2020 13:23:04 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Sep 2020 17:12:41 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 17:12:41 GMT
ENV NATS_SERVER=2.1.8
# Wed, 09 Sep 2020 17:12:42 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 09 Sep 2020 17:12:43 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 09 Sep 2020 17:13:51 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Sep 2020 17:15:26 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Sep 2020 17:15:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Sep 2020 17:15:28 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Sep 2020 17:15:29 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Sep 2020 17:15:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1d56eeebea105bba2dd1879a89adb012f98cf42708c0f36ca4af683db7162a2`  
		Last Modified: Wed, 09 Sep 2020 16:49:22 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4d96d0f21f7d823b426589ab2a404cd548354f8d03ceb98ed43812aa4ea498`  
		Last Modified: Wed, 09 Sep 2020 17:16:52 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9622b50495de28ed9ac7a828c8c525f5d1f3fe10f018169a78a937f320ce673`  
		Last Modified: Wed, 09 Sep 2020 17:16:49 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693bf8afbdb7ba6b5c59a194e3aefcfa41d2ad4c62e07d0961f180475570c386`  
		Last Modified: Wed, 09 Sep 2020 17:16:49 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b791adbede0214cebdc3b0f107e4d8be1105f272f85730e56a9c4bf5d44bed`  
		Last Modified: Wed, 09 Sep 2020 17:16:49 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d5083dfc8cb493d24c2ea383b470122bcff20c1348d9c40c837770030d8628`  
		Last Modified: Wed, 09 Sep 2020 17:16:50 GMT  
		Size: 5.4 MB (5379065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9444d0693ec2f93eb3184f285edbd5be7140a93d9c4309b7133979c5b5e4b34a`  
		Last Modified: Wed, 09 Sep 2020 17:17:03 GMT  
		Size: 13.9 MB (13931410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f0768454035fe701badc16b0bc29578cccb8738206c796ba98b4c1bc44718b`  
		Last Modified: Wed, 09 Sep 2020 17:16:46 GMT  
		Size: 1.7 KB (1681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de26bc51804e14983351214fb629d39bb48d1aab8771e64f000ff4bf51b2268d`  
		Last Modified: Wed, 09 Sep 2020 17:16:46 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74800b43b5c09e14a9ff54d17fac976049b117d63e9ae3e6fdd2855b6cc334c9`  
		Last Modified: Wed, 09 Sep 2020 17:16:47 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92161369e5b87a001a435fffd1802842044b222b30d4fce6964d39a2ab66d896`  
		Last Modified: Wed, 09 Sep 2020 17:16:46 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:68052566a345b1974727afb0e13ccf5da8cd92efabede8c67f188abaabecdac9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats@sha256:1c83509a0dd49bb818407142b5595766fc8cadb59834e72c0a91deaea371ff34
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2369206825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06a6b490bf0f236facc1bf15bf5fbab8a4741401eb02c00e2bf0f129dd66c20d`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Sep 2020 13:15:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Sep 2020 17:10:34 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 17:10:34 GMT
ENV NATS_SERVER=2.1.8
# Wed, 09 Sep 2020 17:10:35 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 09 Sep 2020 17:10:35 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 09 Sep 2020 17:11:05 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Sep 2020 17:12:10 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Sep 2020 17:12:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Sep 2020 17:12:12 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Sep 2020 17:12:13 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Sep 2020 17:12:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1df31adcc7026c3bf0cb32832a3f307dd6e1e54b8b3e050f8a73b5caee674d88`  
		Last Modified: Wed, 09 Sep 2020 16:48:51 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a005485001c0802bc2ee93661375bfb4c868e16c3f5678debf00f29a8bb26386`  
		Last Modified: Wed, 09 Sep 2020 17:16:08 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662e6fbc5f9e16fc0afc4d05927cd1e64bfa92f69d228567abe407bb72908aaf`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7151925f65e3cf12e20bc6f6aa94dfb90b475195bea0a8bd3c8d70d21fe6e7`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf309bd49456f53f290cc9143ca63dc647713cb7981d22d61d7f8b18548b8ae`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fd4c97d4d46deef398e38f156ba05f404a8de7e7f7915b45a96e1b84c98e2e`  
		Last Modified: Wed, 09 Sep 2020 17:16:11 GMT  
		Size: 4.8 MB (4784097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39896e9d43e963384628807bede8a7bea2735860d8797978d74cdccb2db3cccc`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 13.1 MB (13139733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303f12072d6a77ef8f3b35b86cd6fd3a37c88fdd85e2a20d6946ad7fdb5678b4`  
		Last Modified: Wed, 09 Sep 2020 17:16:03 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02cf56909eff26727cabe26c37adb7b07aa76875550f66e267c0e9044d8f19c7`  
		Last Modified: Wed, 09 Sep 2020 17:16:03 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0c7ccbe6779b4f737d7987f4246dc066853208e9957364e0ea8e0d4ee07b47`  
		Last Modified: Wed, 09 Sep 2020 17:16:04 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a250cb3a50140ec9efe6f52457ea634df38df6babd373210cf8c5abb888f7a29`  
		Last Modified: Wed, 09 Sep 2020 17:16:03 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:e0113341e4407f3e09685758839e17a425ac36640e0b8ef2c1b72f61ef0f50ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3930; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.3930; amd64

```console
$ docker pull nats@sha256:281ee36c5f01f3f13192b7d9679e9ae68d89c2efb0d69f3e065fe29832ebc1a7
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5758575718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c71f48677d301c4540845a160ba3f4b3d6b2922f3032940a417555ff8ae48031`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Sep 2020 13:23:04 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Sep 2020 17:12:41 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 17:12:41 GMT
ENV NATS_SERVER=2.1.8
# Wed, 09 Sep 2020 17:12:42 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 09 Sep 2020 17:12:43 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 09 Sep 2020 17:13:51 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Sep 2020 17:15:26 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Sep 2020 17:15:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Sep 2020 17:15:28 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Sep 2020 17:15:29 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Sep 2020 17:15:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1d56eeebea105bba2dd1879a89adb012f98cf42708c0f36ca4af683db7162a2`  
		Last Modified: Wed, 09 Sep 2020 16:49:22 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4d96d0f21f7d823b426589ab2a404cd548354f8d03ceb98ed43812aa4ea498`  
		Last Modified: Wed, 09 Sep 2020 17:16:52 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9622b50495de28ed9ac7a828c8c525f5d1f3fe10f018169a78a937f320ce673`  
		Last Modified: Wed, 09 Sep 2020 17:16:49 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693bf8afbdb7ba6b5c59a194e3aefcfa41d2ad4c62e07d0961f180475570c386`  
		Last Modified: Wed, 09 Sep 2020 17:16:49 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b791adbede0214cebdc3b0f107e4d8be1105f272f85730e56a9c4bf5d44bed`  
		Last Modified: Wed, 09 Sep 2020 17:16:49 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d5083dfc8cb493d24c2ea383b470122bcff20c1348d9c40c837770030d8628`  
		Last Modified: Wed, 09 Sep 2020 17:16:50 GMT  
		Size: 5.4 MB (5379065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9444d0693ec2f93eb3184f285edbd5be7140a93d9c4309b7133979c5b5e4b34a`  
		Last Modified: Wed, 09 Sep 2020 17:17:03 GMT  
		Size: 13.9 MB (13931410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f0768454035fe701badc16b0bc29578cccb8738206c796ba98b4c1bc44718b`  
		Last Modified: Wed, 09 Sep 2020 17:16:46 GMT  
		Size: 1.7 KB (1681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de26bc51804e14983351214fb629d39bb48d1aab8771e64f000ff4bf51b2268d`  
		Last Modified: Wed, 09 Sep 2020 17:16:46 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74800b43b5c09e14a9ff54d17fac976049b117d63e9ae3e6fdd2855b6cc334c9`  
		Last Modified: Wed, 09 Sep 2020 17:16:47 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92161369e5b87a001a435fffd1802842044b222b30d4fce6964d39a2ab66d896`  
		Last Modified: Wed, 09 Sep 2020 17:16:46 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
