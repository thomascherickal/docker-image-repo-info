## `eclipse-temurin:17-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:78a15f679a42e9614bb39e01e686266af69c232c3817a52172f2a0e93fec4981
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `eclipse-temurin:17-nanoserver-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull eclipse-temurin@sha256:f74dbcb4d2e81fef597ce0d99fda11374aebf5bb486469472c0dbf74aae73500
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.7 MB (305716273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2dd94ee0a223223cc88d39b1b5726335d54b49fa596f7a2eed99eed6c18a598`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 08 Jun 2023 12:38:25 GMT
RUN Apply image 10.0.20348.1787
# Wed, 14 Jun 2023 18:10:16 GMT
SHELL [cmd /s /c]
# Wed, 14 Jun 2023 18:12:57 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 14 Jun 2023 18:12:58 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 14 Jun 2023 18:12:59 GMT
USER ContainerAdministrator
# Wed, 14 Jun 2023 18:13:09 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 14 Jun 2023 18:13:10 GMT
USER ContainerUser
# Wed, 14 Jun 2023 18:13:25 GMT
COPY dir:124ac1113930ce4049263b0be6b87edbaf53b403e9545bc9faa31b4eed61cbf5 in C:\openjdk-17 
# Wed, 14 Jun 2023 18:13:40 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 14 Jun 2023 18:13:40 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:f94f5e4cef3f52c830328b87b7298c638fa9ef22a0babf737eda2a2dd6d024c4`  
		Last Modified: Tue, 13 Jun 2023 20:05:48 GMT  
		Size: 120.0 MB (120028549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b91974e610b0adc71baa1c4d1aa6d7a239880c5cef55dc0d33ffd0ef5ac9c14`  
		Last Modified: Wed, 14 Jun 2023 18:36:54 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0863611296cca21816f8f9c468d89f12b6e3ad125edcf355d89f9efd17730c1f`  
		Last Modified: Wed, 14 Jun 2023 18:38:35 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d672dbb96c8308ac75e7cead1fb5d30519d6b608be976168c6e18b9f5bf184`  
		Last Modified: Wed, 14 Jun 2023 18:38:35 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feeeb9494e86c79402d20d5e85bf1653bbeaaf6d7c1cb4c592a46a9a7e2f395e`  
		Last Modified: Wed, 14 Jun 2023 18:38:35 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac8a9f614ab03fa3e4d5204124b782d1d3989700109217154c7bd9ed2394bebe`  
		Last Modified: Wed, 14 Jun 2023 18:38:33 GMT  
		Size: 83.7 KB (83691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bcae215d51b9187a2e9932467054cf98b7b3cfb366cfe04c0d192f0e8dc579f`  
		Last Modified: Wed, 14 Jun 2023 18:38:33 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d614cc07147cce2a4b03b2a8b0221421ca8daf2e3cd80956074be6cf17d308d`  
		Last Modified: Wed, 14 Jun 2023 18:38:52 GMT  
		Size: 185.5 MB (185535594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ab9d2683f5fb23ff888d1c2bebb7405a5563e1792b8fd48ee6d4730647e1ab9`  
		Last Modified: Wed, 14 Jun 2023 18:38:33 GMT  
		Size: 62.2 KB (62211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:401868ecce6163dbf07e6b5f299f3970e88f52132b68d1f98e9f059bc3e6654d`  
		Last Modified: Wed, 14 Jun 2023 18:38:33 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
