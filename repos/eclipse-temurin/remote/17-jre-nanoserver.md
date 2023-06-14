## `eclipse-temurin:17-jre-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:03e6fe9d223f339b94ef9ae2fd97553853087d04432780d6805117788cc1cd8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1787; amd64
	-	windows version 10.0.17763.4499; amd64

### `eclipse-temurin:17-jre-nanoserver` - windows version 10.0.20348.1787; amd64

```console
$ docker pull eclipse-temurin@sha256:2ac09fda536e60c40397df8cd44a31563d5704ce201713c331d9ae1f6586d6cb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.5 MB (163518401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91340d9fcaf67dad7e01deab6fc48b4fe0ea178ea86f5a58007e20d78f88aaaa`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
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
# Wed, 14 Jun 2023 18:13:59 GMT
COPY dir:8912d07424b5206284ef3b7586d69c3f366b527bba3d6f334194ae58c2152641 in C:\openjdk-17 
# Wed, 14 Jun 2023 18:14:12 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
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
	-	`sha256:2c603264f761d27fbacb79e29350b54cd1b48c303d36f7f16d60eb481dac31b1`  
		Last Modified: Wed, 14 Jun 2023 18:39:13 GMT  
		Size: 43.3 MB (43326550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b758e9cff7f7005b742b400b7fd15e6a08bd7825b68a2270133a72a878fe283b`  
		Last Modified: Wed, 14 Jun 2023 18:39:04 GMT  
		Size: 74.4 KB (74415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:17-jre-nanoserver` - windows version 10.0.17763.4499; amd64

```console
$ docker pull eclipse-temurin@sha256:0c6c3bbf66eacb48fe91e80bcbb6594c0998acdbc9c81174c3ec6a6988cb37c9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.8 MB (150831395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26ccfa01bb6157665176c2a93e4ce48b7a991cf37c463e483b128ac387ca45b7`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
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
# Wed, 14 Jun 2023 18:02:13 GMT
COPY dir:8912d07424b5206284ef3b7586d69c3f366b527bba3d6f334194ae58c2152641 in C:\openjdk-17 
# Wed, 14 Jun 2023 18:02:24 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
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
	-	`sha256:670cc69842f65c8edac7311b0ff7af043e2408861faab1f7d36f9d0e90091d29`  
		Last Modified: Wed, 14 Jun 2023 18:33:49 GMT  
		Size: 43.3 MB (43326784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446ccfcedd122ac3b01d6c36e82f1927c9cb4869fadfe95e3f503533567ab689`  
		Last Modified: Wed, 14 Jun 2023 18:33:41 GMT  
		Size: 3.0 MB (3031748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
