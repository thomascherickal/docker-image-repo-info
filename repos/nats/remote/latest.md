## `nats:latest`

```console
$ docker pull nats@sha256:6923c5f75f670dabe310c5dc2d3242e4f9ad4f1eabc625e18716358427ccd8d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2061; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:4f6857e56d3555432c7bc830fb297d8c00cbe3b0522f81dfc8c84a4dacb54ed5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4505352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23830fcc7f9834fd409d95d2bf9877f21b609b7b7392bfcd4b8b5e62e8be14fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:23:05 GMT
COPY file:0b22daa17d88302a2606c64df249d26684c5926e82494be3f08d920922b75196 in /nats-server 
# Mon, 02 Aug 2021 21:23:05 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:23:05 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:23:05 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:23:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:267760e6058167430070f7584ea1e5e18b4ddf538aec80d4b764ba1b9096b403`  
		Last Modified: Mon, 02 Aug 2021 21:23:56 GMT  
		Size: 4.5 MB (4504877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612bea9c73fc6c5c02659a6bff01f1bcada2f4c47323021b03bee52a9ca1eba0`  
		Last Modified: Mon, 02 Aug 2021 21:23:55 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:6e42eec5a210d9a5b6d95c179d5c55193b69846c76786a81908536eac2efbdc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4173716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31e1feb9bf2ac457664507fc7899f48e45d49df93dd60eacdea8b8a9cda8ec51`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:17:15 GMT
COPY file:55e1c39fb6ec9785ddf1c189ad5438b9f306c3e1c2a355512f4efc73aa1aacf6 in /nats-server 
# Mon, 02 Aug 2021 21:17:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:17:16 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:17:16 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:17:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f318c30554fccfe6a5ac8a63f4457a20876b88ede949510db6a8f1c5bcf1442`  
		Last Modified: Mon, 02 Aug 2021 21:19:37 GMT  
		Size: 4.2 MB (4173243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c9419bcd494c007ef4d4f83649e535bb32d84c81337abb67e153ad75a1fb5f`  
		Last Modified: Mon, 02 Aug 2021 21:19:35 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:def02210305c7940addd2f5e26e8417017a2f2ae11116ee001b8f2a7bcb17bff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3992886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20941bb671159cef8cb5d6b9047f5c6c298a495274b06f9c6d9278ea5f9e5a1f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 07 Jul 2021 06:38:20 GMT
COPY file:a259b6f87cc2d22082524e5ba23201057e836734749f0d28676e8637d920d385 in /nats-server 
# Wed, 07 Jul 2021 06:38:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 07 Jul 2021 06:38:21 GMT
EXPOSE 4222 6222 8222
# Wed, 07 Jul 2021 06:38:22 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 07 Jul 2021 06:38:22 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:434fc0c4a6c5daa82c731102728bcac575b5a312862a89edf401b0305d2efc82`  
		Last Modified: Wed, 07 Jul 2021 06:40:42 GMT  
		Size: 4.0 MB (3992410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c195f08925b050ce566763c31c813f3d8c7e1ba40bc4ccdf0949cb87373c3a43`  
		Last Modified: Wed, 07 Jul 2021 06:40:39 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7a367e1495e9df2cf9cc81af565194815e52b37c0ed1fd7e9f278d88311be5b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4120338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad1e0c5709f39238c0ff863c80e1595fb5da12e230643dc6fd4bd6b33cda4039`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:06:28 GMT
COPY file:d94287ad868b49da5d590782f3102415d5dfd4ed2a775b4e4c10280c8ab25db3 in /nats-server 
# Mon, 02 Aug 2021 21:06:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:06:29 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:06:29 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:06:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4ecc856c82596f8b8982843cac0e5ec138e9c881bfd322038cd7cf0f4942c9c9`  
		Last Modified: Mon, 02 Aug 2021 21:07:52 GMT  
		Size: 4.1 MB (4119864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fa4df40d0356fc86fe0d6c780d2a447fe1b2c32b5572c65a3c7d2354961da4`  
		Last Modified: Mon, 02 Aug 2021 21:07:51 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:baf086eb51e7090cb2ef985758c034c882cbe1dd8d4b2a682a618d32b9215e35
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107296331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d57bb9c1561692bbad5576428cd8e22189f1addf3a8b82e73e3f27e246bd485`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 21:17:05 GMT
RUN cmd /S /C #(nop) COPY file:359dd4a92709029cd62dc9620a8ff30527cb3494d6b89c9332ae019bae51b57b in C:\nats-server.exe 
# Mon, 02 Aug 2021 21:17:08 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 02 Aug 2021 21:17:10 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:17:13 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 02 Aug 2021 21:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab54ee8cb88b349708e6f2d10afe13c1d843b9c1ff995a70d40af5ca886eda42`  
		Last Modified: Mon, 02 Aug 2021 21:21:37 GMT  
		Size: 4.6 MB (4564319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d161923a9b16db535efc5f78e4aedd08225387cc8377cedb826e7539fa9051`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e88c4ba846a11b45abc01afc7de665b15430ebfd4c6e585ba8cb11d896017cd`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ca1fda898c73546bdd8f1655f276fe9a0911a7c16f5a4054cdb40e996692c2`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:088b6cb05a147f4faf4e14f0fc1ecda8481f5ad0a8741dba786aebba4374207b`  
		Last Modified: Mon, 02 Aug 2021 21:21:36 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
