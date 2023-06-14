## `eclipse-temurin:8-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:835e5e8872f3295affee0641bd9e8e85cfac1193dd130289a03a1d932ca7550b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `eclipse-temurin:8-nanoserver-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull eclipse-temurin@sha256:c35bc7edd4655732b48763e2eb34214cc76a0c4e714ca7900804247e135a6ba8
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.0 MB (206001614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28cffdfb5de129efb61bd5c97a30f41137ad0f526c9ad8f8367d3286ab841ce2`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 08 Jun 2023 12:28:32 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:41:42 GMT
SHELL [cmd /s /c]
# Wed, 14 Jun 2023 17:41:43 GMT
ENV JAVA_VERSION=jdk8u372-b07
# Wed, 14 Jun 2023 17:41:44 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 14 Jun 2023 17:41:44 GMT
USER ContainerAdministrator
# Wed, 14 Jun 2023 17:41:57 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 14 Jun 2023 17:41:57 GMT
USER ContainerUser
# Wed, 14 Jun 2023 17:42:08 GMT
COPY dir:27c7e47be02cf877d3f45f48fc9f53f313487829869ebfc4770f3f1b0ee2a0d5 in C:\openjdk-8 
# Wed, 14 Jun 2023 17:42:21 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:db019f0eac9dcad0cfd76829e0606fc3759641cb53511bb3535cef61aef4fdcf`  
		Last Modified: Wed, 14 Jun 2023 18:26:46 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7272fe80b4ef0ac5c142d767c7636d470570914eb09cafa7acb9984b6f8ab29`  
		Last Modified: Wed, 14 Jun 2023 18:26:46 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924439698c6ac9e1f4c8e162caf6843a1755893cab4179758aa40c021db2586d`  
		Last Modified: Wed, 14 Jun 2023 18:26:44 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4d176e42bd3de2c765eda8b596b2ef0cf0a6fc0aa32de0848478174ef196d8`  
		Last Modified: Wed, 14 Jun 2023 18:26:44 GMT  
		Size: 69.4 KB (69404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5302d03e13870dffbd24757833957ab84dbeda5c04da418c30766476648b1bee`  
		Last Modified: Wed, 14 Jun 2023 18:26:44 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9045527b618646b0c13d192ec68185ddb40324391a4204cd4fae9a76b1345cb2`  
		Last Modified: Wed, 14 Jun 2023 18:26:58 GMT  
		Size: 101.4 MB (101440396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eccd334d8e55e706d5f8c50570c32c33eda299663c9ebfdf9869361478c7704`  
		Last Modified: Wed, 14 Jun 2023 18:26:44 GMT  
		Size: 88.1 KB (88118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
