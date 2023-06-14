## `eclipse-temurin:17-jdk-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:d8f90b09e2fd018bae139e9d4758d0cfb5ebcaf513a168c490f3730d3bcfca09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1787; amd64
	-	windows version 10.0.17763.4499; amd64

### `eclipse-temurin:17-jdk-nanoserver` - windows version 10.0.20348.1787; amd64

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

### `eclipse-temurin:17-jdk-nanoserver` - windows version 10.0.17763.4499; amd64

```console
$ docker pull eclipse-temurin@sha256:274590f97c7b3add9bb19404a0c8ff6a91507d93efc7a8a8d09ad18ed579b652
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.7 MB (293672206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30aacad568645b5a9d6c95593ebdc936723fd5748315421650a9dea3a3f2a8f5`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 08 Jun 2023 12:28:32 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:41:42 GMT
SHELL [cmd /s /c]
# Wed, 14 Jun 2023 17:58:28 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 14 Jun 2023 17:58:28 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 14 Jun 2023 17:58:29 GMT
USER ContainerAdministrator
# Wed, 14 Jun 2023 17:58:39 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 14 Jun 2023 17:58:40 GMT
USER ContainerUser
# Wed, 14 Jun 2023 17:58:55 GMT
COPY dir:124ac1113930ce4049263b0be6b87edbaf53b403e9545bc9faa31b4eed61cbf5 in C:\openjdk-17 
# Wed, 14 Jun 2023 17:59:10 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 14 Jun 2023 17:59:11 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:234d39d9b188e7f36d5a77b0d54990ea826551314b6703c83aef3ef20b1a7050`  
		Last Modified: Tue, 13 Jun 2023 19:06:23 GMT  
		Size: 104.4 MB (104397895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2364e413270ecc5b57d2596b092fb57b828229b59e810d9f345fc0d31ca535d`  
		Last Modified: Wed, 14 Jun 2023 18:26:46 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d48fb2505311a9973f4fc50f01f7febad4b84461795c12a99a843440fb3b088`  
		Last Modified: Wed, 14 Jun 2023 18:32:24 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cb40a8f6bd15b0a108590f2640aa9ed831515999505a73d71091cbafac60c7`  
		Last Modified: Wed, 14 Jun 2023 18:32:24 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d83e4b96cec8b19a551085dfc76715b54656ad3fed0ebb6b57b19425a6f99f8a`  
		Last Modified: Wed, 14 Jun 2023 18:32:23 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c795320b8cf80accdd28606fbf167537c52aa96aa50dfcb854d943fab77dc79`  
		Last Modified: Wed, 14 Jun 2023 18:32:22 GMT  
		Size: 69.1 KB (69137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e923ef3a8f4e31eea58b06ee6e5cdecb6275cc4dfde7d4fc4e132c51ef5d51e5`  
		Last Modified: Wed, 14 Jun 2023 18:32:21 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7cc8548c19226a90fc68df0d53d624ddde108c8b0d13b9d46a95bf99beb90f`  
		Last Modified: Wed, 14 Jun 2023 18:32:48 GMT  
		Size: 185.5 MB (185537966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87eb21ddf7f719ba60b1ff6a93a61c7b83a4e4cc035c54e9d59e3fce596192ae`  
		Last Modified: Wed, 14 Jun 2023 18:32:23 GMT  
		Size: 3.7 MB (3660215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744a8ba60a5d17502141fe94e78ea667fff4df86da9ee6fb4ab457763df6ef05`  
		Last Modified: Wed, 14 Jun 2023 18:32:21 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
