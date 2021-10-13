## `nats:latest`

```console
$ docker pull nats@sha256:1222b490e96f31013b48932174cea55aa0163f0ebec5a403ebbe03e56603ab52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2183; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:a43c679fb63f49a56f6710d3f4afaef53226518d9433f814f60ce9ea52b7799e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4557856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63a38932d62612b28ddaad81d77d2a01622145f4361d28295cec7f6987c2511d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 24 Sep 2021 18:20:54 GMT
COPY file:56cc63952bfc4b2de2d1c200fd8cbf8f038a5f5f11289a52868a5df2375492b0 in /nats-server 
# Fri, 24 Sep 2021 18:20:54 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 24 Sep 2021 18:20:54 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:20:54 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 24 Sep 2021 18:20:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d16cac695b49a91619219e07a1503c4b96bcbe05f6b920081821c5efd29327e2`  
		Last Modified: Fri, 24 Sep 2021 18:21:47 GMT  
		Size: 4.6 MB (4557381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c945b005f9f3d8bf10851073ef8acbc52c6f2684a073d4068fc6d5b4e5848334`  
		Last Modified: Fri, 24 Sep 2021 18:21:46 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:93693c23ea5644f401a72bf6929214e9dfd2720b1b4c373025e689c1495de5a4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4228700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a1d37c768b08a19ab2b56aff52bc2bd23a18c665a38568b80d03d43b91ebe1d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 12 Oct 2021 23:50:02 GMT
COPY file:87c492688776372ccf80f66cfc3e90fd8fab44035811506c7aaa232e547e000b in /nats-server 
# Tue, 12 Oct 2021 23:50:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 12 Oct 2021 23:50:03 GMT
EXPOSE 4222 6222 8222
# Tue, 12 Oct 2021 23:50:04 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 12 Oct 2021 23:50:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3cd12bdf7a9a23f7457d02e8fc11f170382a386c0eeca79fe881fb322825f1a9`  
		Last Modified: Tue, 12 Oct 2021 23:52:26 GMT  
		Size: 4.2 MB (4228225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d6a7556bfb5d88c2ff5e698fcd012e06a282a35550cc4944de84fe772a4481`  
		Last Modified: Tue, 12 Oct 2021 23:52:23 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:d2e70b8a1a863ae0f789502434cef995627ed0f46f551f291f2f7a0ff7017642
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4213288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3787a15077edfb6d8fa1646ed439c24cc005849fcf8311a629d20c8679d8b139`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 30 Sep 2021 19:47:57 GMT
COPY file:6d69eef0d821da908da152f3dfe853b07d173db35f1c40a85e545d8218aaeb7e in /nats-server 
# Thu, 30 Sep 2021 19:47:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 30 Sep 2021 19:47:58 GMT
EXPOSE 4222 6222 8222
# Thu, 30 Sep 2021 19:47:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 30 Sep 2021 19:47:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c67bb3b32b6353245cbd27e1ee30c47b5cf8b7c76346ca37875fa7cc7086cf7e`  
		Last Modified: Thu, 30 Sep 2021 19:50:22 GMT  
		Size: 4.2 MB (4212814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065d109fdaff0adc51732a8f449fee6ffda396a8e2a53cda9273482aa1fb36f0`  
		Last Modified: Thu, 30 Sep 2021 19:50:19 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:2475df2d82899c998486ff164f63c549ab94f3ec9d6b6ced5f1a828feb097cbb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4170004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dd70c0c61ec57441666601ccff002d189c00d3ecb3a1eb1ea97f052736bee1b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 24 Sep 2021 17:40:34 GMT
COPY file:9b757ffadeb4943a3ca6c78d9caf65891c08587f5bebf5be32974d1456afb89e in /nats-server 
# Fri, 24 Sep 2021 17:40:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 24 Sep 2021 17:40:35 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:40:35 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 24 Sep 2021 17:40:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7d0e0caa3737fe1355285d221e0c8e078337a45e1506022ffc37197d044d1db3`  
		Last Modified: Fri, 24 Sep 2021 17:41:58 GMT  
		Size: 4.2 MB (4169531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f509df5c28970b2ba96c7084c68158896b7fcbf5faf2d170a8d8e61960294c8`  
		Last Modified: Fri, 24 Sep 2021 17:41:57 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats@sha256:71c153413bf49b38806c3ad0c2a85c117380534d5d8587c9e930ad7061197323
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107323878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8917f61d9feda334e63e3bb8a7406359fccecff0aacc392edaf7b993af8e1f33`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 13 Sep 2021 03:45:12 GMT
RUN Apply image 1809-amd64
# Wed, 15 Sep 2021 15:43:05 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 24 Sep 2021 18:18:25 GMT
RUN cmd /S /C #(nop) COPY file:e8e5cb48daba80f34796952e26cc4058ca5809e456780e196277b4f6b98248b9 in C:\nats-server.exe 
# Fri, 24 Sep 2021 18:18:26 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 24 Sep 2021 18:18:27 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:18:28 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 24 Sep 2021 18:18:28 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3585a81ca503e6c63dce938a5606f4171d7461e51000a92054b3f5692786d6c9`  
		Size: 102.7 MB (102703785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:66dbf96361e9ec1f64f66e255a947eab476edef46c3f9a3b4ede943fa8b87699`  
		Last Modified: Wed, 15 Sep 2021 15:46:11 GMT  
		Size: 1.1 KB (1089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a89e42bde9eba1e3c234a1b0fa3c923f6980959a141c870e6d8b49353b89c52`  
		Last Modified: Fri, 24 Sep 2021 18:22:59 GMT  
		Size: 4.6 MB (4613776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef71520d14dc0a4fa2ff138a03b2e1cba90e07a07e5d8a4095bf4939e740ecb4`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.8 KB (1759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd964bd5c073449877455885b3d3466daa9f611ce0979ea4c4fd13f8d586721`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f529e09f796786e8eefc1792f39c3dcad6a7fb167fa5ead20c40310f632810`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a619e9f3c2ad169084d8726e34725b9a6f47e3a0cbc88a2433a04b76b32e23`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
