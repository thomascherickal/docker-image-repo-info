## `eclipse-temurin:11-jre-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:571d8bdf08b3c209455adf3b44b562e184497dfd5dbf194f140852018a925173
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1787; amd64
	-	windows version 10.0.17763.4499; amd64

### `eclipse-temurin:11-jre-nanoserver` - windows version 10.0.20348.1787; amd64

```console
$ docker pull eclipse-temurin@sha256:bae1850529fa97b4f17f7ca4ea001f727290f5021cf285e5e99c3ff4e2b42eab
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.4 MB (163364913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3fbc45d620055810ed13da61dd9ea943f7fde1225f9a5556450d481711f3ba3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
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
# Wed, 14 Jun 2023 18:12:36 GMT
COPY dir:b6e5aca1f3f361bc79d6ed078f0846fae24cf0b7748963379a92b2a6511b98d8 in C:\openjdk-11 
# Wed, 14 Jun 2023 18:12:48 GMT
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
	-	`sha256:5ef1f8867be2480b0448e41f49874aa489967c34e288afebf1e815db331f9040`  
		Last Modified: Wed, 14 Jun 2023 18:38:24 GMT  
		Size: 43.2 MB (43164603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b60c22841603f21d8593f846f0e4e67e5cfe8f6716758d2a3d3ff53822147114`  
		Last Modified: Wed, 14 Jun 2023 18:38:16 GMT  
		Size: 73.0 KB (73041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-jre-nanoserver` - windows version 10.0.17763.4499; amd64

```console
$ docker pull eclipse-temurin@sha256:302e075b327d7f26d84e6817272d8853db8e328f320edb5c17456e508951fac9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.7 MB (147711880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69295adc084a69c3f3e90c3637065b7141bf008a9c2bd632f070741d11ed2065`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
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
# Wed, 14 Jun 2023 17:54:01 GMT
COPY dir:b6e5aca1f3f361bc79d6ed078f0846fae24cf0b7748963379a92b2a6511b98d8 in C:\openjdk-11 
# Wed, 14 Jun 2023 17:54:25 GMT
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
	-	`sha256:8d5e71b0449e1754a9ab4b45f29e2551beb770bd8ac1517c1949e794e23a2b85`  
		Last Modified: Wed, 14 Jun 2023 18:30:54 GMT  
		Size: 43.2 MB (43157629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d29a6d32ca19e64ee4ce7b1dfbd02226b70d056aa8759c8fe0f050e214b052ad`  
		Last Modified: Wed, 14 Jun 2023 18:30:45 GMT  
		Size: 81.8 KB (81835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
