## `openjdk:21-ea-27-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:8dfe28d19e67d311a43d5a787748ba2d1329ad46a8b719d566f4811b26e4d2d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `openjdk:21-ea-27-jdk-nanoserver` - windows version 10.0.17763.4499; amd64

```console
$ docker pull openjdk@sha256:e7fd142b92ab191b64336bec7ea38c296c16c8d469bbbf7a13eae2ccff172859
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.2 MB (306231415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:953f084f5bdab4a2d3e5f653c904d88314ee857ea857a9f11965011d7731a67b`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 08 Jun 2023 12:28:32 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:41:42 GMT
SHELL [cmd /s /c]
# Wed, 14 Jun 2023 20:32:10 GMT
ENV JAVA_HOME=C:\openjdk-21
# Wed, 14 Jun 2023 20:32:11 GMT
USER ContainerAdministrator
# Wed, 14 Jun 2023 20:32:20 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 14 Jun 2023 20:32:21 GMT
USER ContainerUser
# Wed, 21 Jun 2023 01:59:21 GMT
ENV JAVA_VERSION=21-ea+27
# Wed, 21 Jun 2023 01:59:37 GMT
COPY dir:ed79e275a6c79de44d26d4dc06a4f25677470766d38a05ba2765882877fb8229 in C:\openjdk-21 
# Wed, 21 Jun 2023 01:59:51 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Wed, 21 Jun 2023 01:59:51 GMT
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
	-	`sha256:a9c86c8f72d5c620385f29493830932257c53d9dad74802ecdf0bdbc03b2494c`  
		Last Modified: Wed, 14 Jun 2023 20:37:08 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30698f58bfeb99d6b9b76177da8956540b4b318293543c1e5c8447403dc97f1`  
		Last Modified: Wed, 14 Jun 2023 20:37:08 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c50e91142bca7a5ff55e1ebc6fd6e7a26cdfc9d0890ad2eb8a5c7b031598294`  
		Last Modified: Wed, 14 Jun 2023 20:37:08 GMT  
		Size: 68.8 KB (68836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a22e7e5b49f87fd9c56f26a1e630fdf989e0f48edc7f35e074d47642e4af389`  
		Last Modified: Wed, 14 Jun 2023 20:37:06 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64d275ccaf08ff04f681c6a70a160ebd75c557e2680c91523bb962c17ae39c7`  
		Last Modified: Wed, 21 Jun 2023 02:04:29 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6208bce939c7d49a06ba56ddc2323a516838d0fe0d4e326439e3cde5eeee7f9b`  
		Last Modified: Wed, 21 Jun 2023 02:04:50 GMT  
		Size: 198.0 MB (197954494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a88751904447b306faf4f46b8c4721f7c601e102c257225ccc878d65d6ba94`  
		Last Modified: Wed, 21 Jun 2023 02:04:30 GMT  
		Size: 3.8 MB (3803199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4988f821de35bc7420a924085ed7249dfeb1839cc649edf7ebaa3e20f79a7bc`  
		Last Modified: Wed, 21 Jun 2023 02:04:29 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
