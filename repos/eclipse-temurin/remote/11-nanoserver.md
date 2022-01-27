## `eclipse-temurin:11-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:54fe88cba2caee23e6eeb8af0914bb8d9c5e3eefc10a89850313bc83c831df06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.473; amd64
	-	windows version 10.0.17763.2458; amd64

### `eclipse-temurin:11-nanoserver` - windows version 10.0.20348.473; amd64

```console
$ docker pull eclipse-temurin@sha256:b0cd2116b93a67f0ea1e8de4f5a25aff17af96e942dea99b3afb164226b08501
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.4 MB (309446425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e30c63a85252be4bc2b73a3f8ebf22f7e0d472aa266167f7a44e19a9f4eb2f14`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sun, 16 Jan 2022 04:54:46 GMT
RUN Apply image ltsc2022-amd64
# Wed, 26 Jan 2022 19:40:03 GMT
SHELL [cmd /s /c]
# Wed, 26 Jan 2022 19:41:56 GMT
ENV JAVA_VERSION=jdk-11.0.13+8
# Wed, 26 Jan 2022 19:41:56 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 26 Jan 2022 19:41:57 GMT
USER ContainerAdministrator
# Wed, 26 Jan 2022 19:42:15 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 26 Jan 2022 19:42:16 GMT
USER ContainerUser
# Wed, 26 Jan 2022 19:42:49 GMT
COPY dir:7549fd743977f7762910679960e9adfeab116385590a40bc0f1570100fce1af1 in C:\openjdk-11 
# Wed, 26 Jan 2022 19:43:06 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 26 Jan 2022 19:43:07 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:7691725ee3658d154f940d82fd8c3ff07c0dc589a0c9a93df47ed0ede92a76ab`  
		Size: 117.3 MB (117333150 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f9f8c9f771ab6c67c92a4cbe90414c7b9311902f2b42d89abf566df9ac29c8df`  
		Last Modified: Wed, 26 Jan 2022 20:24:57 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01b41410fc03954f41e9ffc0f1393a3fcacfe4d5753730349d81020f3056e4f`  
		Last Modified: Wed, 26 Jan 2022 20:25:41 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:effda956ec85bcc291bbd87bb22c44f2d1d663998261ffa0464a1b0ed2cf0074`  
		Last Modified: Wed, 26 Jan 2022 20:25:41 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0befa22568433dd705424450fb284e00b461460d86fb537b1155d3bcd088cc0`  
		Last Modified: Wed, 26 Jan 2022 20:25:41 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea6dcba2f2eadef2624cd779a242cd2e480054b039bdca1a226654f7426318a`  
		Last Modified: Wed, 26 Jan 2022 20:25:39 GMT  
		Size: 82.7 KB (82709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7376345a2cdc83d6f0c658965896b7354ec6b6a8fcdd9aa191f4fc226d3d962a`  
		Last Modified: Wed, 26 Jan 2022 20:25:39 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd00707d32afdde6d9b37508b5113e0b1a3924fa86ada601d90078d49a0e5f9`  
		Last Modified: Wed, 26 Jan 2022 20:29:25 GMT  
		Size: 191.9 MB (191926621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19ea0690ec3b6bbf1b60d504d50f3089991c4631ee32b00ddba917e07e78433`  
		Last Modified: Wed, 26 Jan 2022 20:25:39 GMT  
		Size: 97.1 KB (97057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4e2fea354286e8e5897ebceacd63ef52856e5aa5003afd3967b9ad882c8377`  
		Last Modified: Wed, 26 Jan 2022 20:25:39 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-nanoserver` - windows version 10.0.17763.2458; amd64

```console
$ docker pull eclipse-temurin@sha256:bf3381e8b97d4a56805ddd8773ade92167ac1922e66a5ade9b0d817908e4af2f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.2 MB (295150114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8071aa54074e48358c1e57e494fe0e473e5079c3f3548bb982a25300212bea0`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 19 Jan 2022 22:25:45 GMT
SHELL [cmd /s /c]
# Wed, 26 Jan 2022 19:15:36 GMT
ENV JAVA_VERSION=jdk-11.0.13+8
# Wed, 26 Jan 2022 19:15:37 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 26 Jan 2022 19:15:37 GMT
USER ContainerAdministrator
# Wed, 26 Jan 2022 19:16:01 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 26 Jan 2022 19:16:01 GMT
USER ContainerUser
# Wed, 26 Jan 2022 19:16:34 GMT
COPY dir:7549fd743977f7762910679960e9adfeab116385590a40bc0f1570100fce1af1 in C:\openjdk-11 
# Wed, 26 Jan 2022 19:16:50 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 26 Jan 2022 19:16:51 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b5c97e1d373f591225559869af7f4f01399c201f89d21f903b1d23c830aa0a3f`  
		Size: 103.0 MB (103046552 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a1b3e13bb7b3d4b61b5f49a91d6eb9bfcf5539ab89c3687d608f17713c2409b5`  
		Last Modified: Thu, 20 Jan 2022 02:21:30 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123ab2ee14a125bf4b0c6cbaa7024d6fd79d88b72564d3f5ffc2a991388ca55d`  
		Last Modified: Wed, 26 Jan 2022 20:05:11 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22a2e9edcceaff9bcf83e6afe158f5653cb569791bf57461c14bb12dee4c4f4`  
		Last Modified: Wed, 26 Jan 2022 20:05:11 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fd6c39c776fbc28c7dc393f112bb0ec49b97e64c79c5001c3b4c9067461568`  
		Last Modified: Wed, 26 Jan 2022 20:05:11 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5ed98fdccc969f48e18c637043dc0f01001d2592b60ead2a792c7d37dd616c`  
		Last Modified: Wed, 26 Jan 2022 20:05:08 GMT  
		Size: 75.3 KB (75305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c4cf8478e4d4c0f8a13f4a6039564552580a3c553158a2405cac2386232588`  
		Last Modified: Wed, 26 Jan 2022 20:05:08 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f02d23c2d10a747d00a6b7a0e5e13b702809294d12f58f54c9d6776ee2f95c`  
		Last Modified: Wed, 26 Jan 2022 20:05:29 GMT  
		Size: 191.9 MB (191924843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b990ad10118e7f8c6259084d9922c6af0deb76192cc2c2d17548928d8b0ee84c`  
		Last Modified: Wed, 26 Jan 2022 20:05:08 GMT  
		Size: 96.5 KB (96480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a7e9ed5a78c20ee9aaa8d114201b7782b58e5b36344380adb35c73aa77a50fd`  
		Last Modified: Wed, 26 Jan 2022 20:05:08 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
