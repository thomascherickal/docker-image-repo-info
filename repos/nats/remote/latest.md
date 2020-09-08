## `nats:latest`

```console
$ docker pull nats@sha256:c839cb9eca783e82eeb8801caa15f37e0e5c6ee3d39fb4fc77f53ed5ae0e1f08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1397; amd64

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

### `nats:latest` - windows version 10.0.17763.1397; amd64

```console
$ docker pull nats@sha256:eeb359a0ca361f7a2ff730023bca6bcdddd0ca0d1412e87554a9360f1fad5c9d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105027949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:262a266c1062a81eb67f96245b8b6dea8e7b0008705ce7051e8783785ff68076`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 06 Aug 2020 01:28:42 GMT
RUN Apply image 1809-amd64
# Wed, 12 Aug 2020 15:13:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 04 Sep 2020 19:46:30 GMT
RUN cmd /S /C #(nop) COPY file:0b6475b59bf6bfe6c1030fd41ea501af74fd46ae70fd98c58683b35f8ed498ff in C:\nats-server.exe 
# Fri, 04 Sep 2020 19:46:31 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 04 Sep 2020 19:46:32 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 04 Sep 2020 19:46:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 04 Sep 2020 19:46:33 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ce1c649a3e5b5b5449776d4afce631c673cade12336ccb5a38a0aac7c9d8b2bc`  
		Size: 101.0 MB (100984944 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b07499a9e4ee2f1cb045788b6e555000daa9000613380cb70f067c5287b55a61`  
		Last Modified: Wed, 12 Aug 2020 15:17:30 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d4dc8c52ad1ff0fc383e64c11688e98d786a5f5409e1367d05cdb80b2db887`  
		Last Modified: Fri, 04 Sep 2020 19:50:48 GMT  
		Size: 4.0 MB (4037963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d6dd2505c3f76661a7f8f43bd3c5bbace4158d66914091710d55ac929b69b44`  
		Last Modified: Fri, 04 Sep 2020 19:50:47 GMT  
		Size: 1.5 KB (1515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51eb47d1ef65e0d4d95aca8e6874ce099026a2626edfe488ef880b5bc19f4102`  
		Last Modified: Fri, 04 Sep 2020 19:50:47 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ecc4c9a56ef41700f167e7f35a916684fc48167e7bd100072d6760e0ae166a9`  
		Last Modified: Fri, 04 Sep 2020 19:50:46 GMT  
		Size: 859.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eaf2a3d43bcc4b2832d9401813b736136a6e81ad7bca4cdcd59d66bdfeb5ff1`  
		Last Modified: Fri, 04 Sep 2020 19:50:47 GMT  
		Size: 933.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
