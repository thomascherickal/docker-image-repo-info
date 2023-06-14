## `eclipse-temurin:11-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:a38618680af92408a96bc0aad2578fee4707ebc3aea49fe6a3540d16502936c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `eclipse-temurin:11-nanoserver-1809` - windows version 10.0.17763.4499; amd64

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
