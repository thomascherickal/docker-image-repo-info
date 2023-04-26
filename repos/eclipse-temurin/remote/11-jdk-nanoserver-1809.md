## `eclipse-temurin:11-jdk-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:2b32098df3d15e02f2e4a74d63a76239a7ab09f45dc3615d0d1885a480e8fda1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `eclipse-temurin:11-jdk-nanoserver-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull eclipse-temurin@sha256:26fbe9fa98c457b3e3eab8bb64842a1a88788d0730a206c7357cac08c729d6f0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.9 MB (299930506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb7eb19848e1f5525b32be5e5af30aa742495319e41323aec3849c149cfc976c`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Tue, 11 Apr 2023 23:45:41 GMT
SHELL [cmd /s /c]
# Wed, 26 Apr 2023 19:28:44 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Wed, 26 Apr 2023 19:28:45 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 26 Apr 2023 19:28:45 GMT
USER ContainerAdministrator
# Wed, 26 Apr 2023 19:28:54 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 26 Apr 2023 19:28:54 GMT
USER ContainerUser
# Wed, 26 Apr 2023 19:29:07 GMT
COPY dir:aa85dc89894032bdcf98e5da06633e8de4813537c791ddbe3fc8bdfa8596f8de in C:\openjdk-11 
# Wed, 26 Apr 2023 19:29:18 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 19:29:18 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:af799fb2ff133c89311c6a42d34b8cb6c9b11d775f52e04ab08389d05e64ed1c`  
		Last Modified: Wed, 12 Apr 2023 00:53:10 GMT  
		Size: 106.8 MB (106788951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1db438f20b81fe0c031e4e3eee58d278fba7258d01057ff18964cccf70d41c`  
		Last Modified: Wed, 12 Apr 2023 00:52:38 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce4e3b8bac3b5d03c157f45ff3320441042109d47d3c0da2bc3a194fe9ad5d2`  
		Last Modified: Wed, 26 Apr 2023 20:02:50 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bcefac68112b666cf61ad6362f369d8237f25f4ee5909e378f8a13fcc4c9fa7`  
		Last Modified: Wed, 26 Apr 2023 20:02:50 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1cad6c030895845be45eeba53c24091757fc1b01db3496ab4752ba176033a6`  
		Last Modified: Wed, 26 Apr 2023 20:02:50 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714f5674d7b5a34fb8f58301a6da94389dc78a251455c2187934ec36d475bbc5`  
		Last Modified: Wed, 26 Apr 2023 20:02:48 GMT  
		Size: 68.5 KB (68504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66362b7ce52315d1faed7636cd5df8b075c26119726a777008f0c74958639b8`  
		Last Modified: Wed, 26 Apr 2023 20:02:48 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e707e684beed80e4b22c7a682e7e0f17e37796dce1bda21391b4cdbdd35a6227`  
		Last Modified: Wed, 26 Apr 2023 20:03:05 GMT  
		Size: 193.0 MB (192983967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1101ddabd1885e7bc5c344310ea69ec4b82f4739ff9b0808ef25bcca70d5596`  
		Last Modified: Wed, 26 Apr 2023 20:02:48 GMT  
		Size: 82.2 KB (82192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88f7d826a7943254265697d6d168a4facc50ecde69abdcbbb9eae4d242063509`  
		Last Modified: Wed, 26 Apr 2023 20:02:48 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
