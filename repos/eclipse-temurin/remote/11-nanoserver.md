## `eclipse-temurin:11-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:db0f1714c9eb041ad3536d0d1a078f2630015382817dd6cc17b16c1321fce90b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1787; amd64
	-	windows version 10.0.17763.4499; amd64

### `eclipse-temurin:11-nanoserver` - windows version 10.0.20348.1787; amd64

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

### `eclipse-temurin:11-nanoserver` - windows version 10.0.17763.4499; amd64

```console
$ docker pull eclipse-temurin@sha256:33737e77601d7d99dd39d91853a330053687e520b6c1f51ef273d08df8374c54
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.5 MB (297547367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78319396eec61f958cce7fae9ef5b0c2650e8f86d8d428365eceac80f782d990`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 08 Jun 2023 12:28:32 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:41:42 GMT
SHELL [cmd /s /c]
# Wed, 14 Jun 2023 17:49:15 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Wed, 14 Jun 2023 17:49:15 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 14 Jun 2023 17:49:16 GMT
USER ContainerAdministrator
# Wed, 14 Jun 2023 17:49:26 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 14 Jun 2023 17:49:26 GMT
USER ContainerUser
# Wed, 14 Jun 2023 17:49:42 GMT
COPY dir:aa85dc89894032bdcf98e5da06633e8de4813537c791ddbe3fc8bdfa8596f8de in C:\openjdk-11 
# Wed, 14 Jun 2023 17:49:57 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 14 Jun 2023 17:49:58 GMT
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
	-	`sha256:773b85913a8d12aa102d9caa16e83b77558077295a82f4bc0c33d34548e9899d`  
		Last Modified: Wed, 14 Jun 2023 18:29:34 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c27d316d64beecf85e742aa27944d0e526dc819642d723d311ccc30f96e85c68`  
		Last Modified: Wed, 14 Jun 2023 18:29:34 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cd6db8526aaff1fe3edfcbb051c1684da77cf7535f7ff7574054d1aa5d4e27`  
		Last Modified: Wed, 14 Jun 2023 18:29:34 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea7668429d10f9bf0b6ff482341c9066b2be7214242417d81645c283bf9bd15b`  
		Last Modified: Wed, 14 Jun 2023 18:29:32 GMT  
		Size: 68.8 KB (68776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558300ef6559266ec31a31947e706bb9a1ba4282295a7bf983c6795989a10135`  
		Last Modified: Wed, 14 Jun 2023 18:29:32 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74bd559c217c09f65aa7631effab042d13c53694c07829e75ec9f0d7c0e08bf3`  
		Last Modified: Wed, 14 Jun 2023 18:29:52 GMT  
		Size: 193.0 MB (192983968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb4dd6ecdbf6155e4265f92aeaec770c2b852423501e30ed1661d9b9987a884`  
		Last Modified: Wed, 14 Jun 2023 18:29:32 GMT  
		Size: 89.8 KB (89849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0df8a63cf3f19c1525b87963b912fffbad4017da758cbba28cbe1ae5fa85507`  
		Last Modified: Wed, 14 Jun 2023 18:29:32 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
