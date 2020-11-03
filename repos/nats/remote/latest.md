## `nats:latest`

```console
$ docker pull nats@sha256:88b648a4f3434e970f17d1fbf34c0c44b7e9256eb072992f2956e7cdd08ec8af
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
$ docker pull nats@sha256:679524b91e0a1e4b983d20d70f7a1495f1c16247cf568f29cbf88f5c4b25e914
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4098136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95713166e2236aefedbb92b1d1ef989f979e5c737ff5c14d45d9e32803f032bb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:32:02 GMT
COPY file:e0a0cbd14b84d81f9a3d73a7eefe99693215eb890370f9aba1b574d4cbf63b52 in /nats-server 
# Tue, 03 Nov 2020 00:32:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:32:03 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:32:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:32:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2d6c7151b0c792ecf790fde24412769bf193e4c1922c8a508f8e137d292b4179`  
		Last Modified: Tue, 03 Nov 2020 00:32:35 GMT  
		Size: 4.1 MB (4097661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b920bf257e35e5e325af3ffc17a4baed7903a77f327e8ec3021f94016a78a239`  
		Last Modified: Tue, 03 Nov 2020 00:32:35 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:7c6e8cffea7e48d3ee02b22fb93947963731051dcc56f3c8ec98f2260768814b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3817067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a584107a14f067c0a007db6f0e42b3ff0c190fa2d866f5581552cc559a035125`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Nov 2020 23:53:40 GMT
COPY file:4cd9814103fc39d1b5bf81e4e528b12e56d59d0efda223c50a7ea420e6d4b421 in /nats-server 
# Mon, 02 Nov 2020 23:53:40 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Nov 2020 23:53:41 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Nov 2020 23:53:41 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Nov 2020 23:53:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e162374a08bbb575088c1eaffc753891ab6589b134493a9f8ba1b148e20f8dec`  
		Last Modified: Mon, 02 Nov 2020 23:54:20 GMT  
		Size: 3.8 MB (3816591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77a00778e9ed2ae19795da75b6f12f291e70490f03cc4565c407af242ace47`  
		Last Modified: Mon, 02 Nov 2020 23:54:20 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:1f4b725d1989c235e10f362b0f9c04a708fe6b1dfb22e2efc236b0d2a001ef8b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3813415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:483d6781ef03c3263effcb9f73ae01394a0dae4af477e75c00c19544d0bfe66b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:03:52 GMT
COPY file:0513d05e9f97918c0430b076865e30771904270865892c092e15d1beb98d08c4 in /nats-server 
# Tue, 03 Nov 2020 00:03:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:03:53 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:03:54 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:03:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ed0e6ae1888bfc5be9efcd3bbca71bd2840e4361003c98476fd25ce7d6e9ee14`  
		Last Modified: Tue, 03 Nov 2020 00:04:34 GMT  
		Size: 3.8 MB (3812940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b242a83395577c4be465d49aee9b3d407ea026cb0383e18836fb6ed16caa34c`  
		Last Modified: Tue, 03 Nov 2020 00:04:33 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:670bb4f03b559b3f9d0d2e736450bbb77ae1a789bbfac3b11a09c531d6cf412e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3795291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd733d2cc8ad31f06df9779323962d0e6f73681100397d3090b1e57bc25be709`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:21:37 GMT
COPY file:e1e30af7043f9127562e3a3ea4612aaf12d52aac32a8466b822dbbbeebaaef76 in /nats-server 
# Tue, 03 Nov 2020 00:21:37 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:21:38 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:21:39 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:21:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6433bc19867b0af777bb4176a307bfb021a5ee3d3ad8390bb912e6787b729c8`  
		Last Modified: Tue, 03 Nov 2020 00:22:16 GMT  
		Size: 3.8 MB (3794815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d0ed92b996d8a726daa5da839bd0dfa4651c38c36a2f9a62af31ed304b10a6`  
		Last Modified: Tue, 03 Nov 2020 00:22:14 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.1518; amd64

```console
$ docker pull nats@sha256:3b8d6e0b7c69852dc23b45a96fef7142a8af7be8283756ed974c14f58e297291
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.3 MB (105252874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3f5cc81e8fe22627c10e8a8c0e8c031081c1422b5fa7a1b9e0d6376a4df1600`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 30 Sep 2020 11:25:56 GMT
RUN Apply image 1809-amd64
# Wed, 14 Oct 2020 16:26:27 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 03 Nov 2020 00:20:01 GMT
RUN cmd /S /C #(nop) COPY file:1bed18dba32dca3cc37e8d20c1b6b2b5179bbc92f869531591951b440efda07a in C:\nats-server.exe 
# Tue, 03 Nov 2020 00:20:02 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 03 Nov 2020 00:20:03 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:20:03 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 03 Nov 2020 00:20:04 GMT
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
	-	`sha256:a832cb76fb4365aa1898af094abe8919525832b45cff3095989d35854e50266d`  
		Last Modified: Tue, 03 Nov 2020 00:24:20 GMT  
		Size: 4.0 MB (4042693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30d14e997b712ff68025da8149e86cb4e26053db26f63189bb11be34d9c4570`  
		Last Modified: Tue, 03 Nov 2020 00:24:19 GMT  
		Size: 1.5 KB (1484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a5619f119bfa73b08a55556d063fe6774602e03b6694241acdf544d8877e81`  
		Last Modified: Tue, 03 Nov 2020 00:24:18 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5eaf47aa7239eb1b644c54510809eb1fac633a32d7472f6eaed679c9016fee0`  
		Last Modified: Tue, 03 Nov 2020 00:24:19 GMT  
		Size: 879.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2638a3eddd847bb58e977d2986b5fea2b056b1ce34e1c991ea6686a340621a69`  
		Last Modified: Tue, 03 Nov 2020 00:24:18 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
