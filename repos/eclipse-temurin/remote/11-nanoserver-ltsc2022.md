## `eclipse-temurin:11-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:8f94b6c270900d3ab83fae78a31fd0cd74e894c614031eac3ddb8b8e4f976f24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `eclipse-temurin:11-nanoserver-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull eclipse-temurin@sha256:8b5afaed1e44064175629bd54a6444292f4cd8fa8e98254e3ecf8d3ca6475220
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.2 MB (313185237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4acd567bafc733ce67d4f1dc395f4913cf2fb62ec456a96102b1902ca6b2a3ae`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 08 Jun 2023 12:38:25 GMT
RUN Apply image 10.0.20348.1787
# Wed, 14 Jun 2023 18:10:16 GMT
SHELL [cmd /s /c]
# Wed, 14 Jun 2023 18:11:35 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Wed, 14 Jun 2023 18:11:36 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 14 Jun 2023 18:11:37 GMT
USER ContainerAdministrator
# Wed, 14 Jun 2023 18:11:46 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 14 Jun 2023 18:11:47 GMT
USER ContainerUser
# Wed, 14 Jun 2023 18:12:04 GMT
COPY dir:aa85dc89894032bdcf98e5da06633e8de4813537c791ddbe3fc8bdfa8596f8de in C:\openjdk-11 
# Wed, 14 Jun 2023 18:12:18 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 14 Jun 2023 18:12:18 GMT
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
	-	`sha256:ed7bfb9c89a190d09d4a3f1ece282adf02829501409f983fe745fad78cbfd6d2`  
		Last Modified: Wed, 14 Jun 2023 18:37:46 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224752ff24c4a1aae224b0c638ee6a94177a06f5e567d5fa5b75cfd3f62c8b1a`  
		Last Modified: Wed, 14 Jun 2023 18:37:46 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69284cf6fc50bc605f5c3b904cb7f07bd114d423c4690b87ad94624d32e44b90`  
		Last Modified: Wed, 14 Jun 2023 18:37:46 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e93af9c5a0cb318d0c915ab07807483261c5c17e313eef532a7d37397a16710`  
		Last Modified: Wed, 14 Jun 2023 18:37:44 GMT  
		Size: 93.2 KB (93195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5998fd7aaea292e132c0b142a42b69c725e507744f99d55c1fd9d1c551cbd807`  
		Last Modified: Wed, 14 Jun 2023 18:37:44 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9abda38c6d7525e8a710edf34d2f2712c95e79ec8cc64a704246a6c0bfc6c7b`  
		Last Modified: Wed, 14 Jun 2023 18:38:04 GMT  
		Size: 193.0 MB (192983847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fbba590899afece5a30252d760a827be516bd90367cadb0c9a049f36576882`  
		Last Modified: Wed, 14 Jun 2023 18:37:44 GMT  
		Size: 73.1 KB (73066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4efcf02014f9afd4547b8a2345ade00b1879e08646dfae50f5763e3d7497f5be`  
		Last Modified: Wed, 14 Jun 2023 18:37:44 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
