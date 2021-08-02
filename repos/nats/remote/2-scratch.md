## `nats:2-scratch`

```console
$ docker pull nats@sha256:7f7c8490b07669dd0f657fed80801af5c91f218bfa2a670269c9970844ccb806
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

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

### `nats:2-scratch` - linux; arm variant v6

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

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:b62db1bffb32e6ee14a5f31627490ee42a7ce9ef23a4dc4a35d4a6369f4a20f9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4168315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f558bfa7884cef624790ee0f5aeee6d6d951906aba1aea71ad8ec6c8dae7f79`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Aug 2021 21:29:15 GMT
COPY file:53e75c3b9678692c71b57cd36d27eaf59bf88a2243c2e393c89e449b7fbbeec4 in /nats-server 
# Mon, 02 Aug 2021 21:29:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Aug 2021 21:29:16 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Aug 2021 21:29:17 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Aug 2021 21:29:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:70efc6c9a421fda065ea73767dddd939851b57c6d56074655d6d5b7e630228c7`  
		Last Modified: Mon, 02 Aug 2021 21:31:40 GMT  
		Size: 4.2 MB (4167841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a1b76009f9d8b59e13cc16f24591c5ae4241d6fff97203d24ece18fa0fe2e3`  
		Last Modified: Mon, 02 Aug 2021 21:31:37 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

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
