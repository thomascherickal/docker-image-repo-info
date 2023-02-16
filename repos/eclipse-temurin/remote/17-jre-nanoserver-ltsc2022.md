## `eclipse-temurin:17-jre-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:60623a7abb923bcc0df353d408abe7e25778d35045a9b9478874aee2e735a76c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1547; amd64

### `eclipse-temurin:17-jre-nanoserver-ltsc2022` - windows version 10.0.20348.1547; amd64

```console
$ docker pull eclipse-temurin@sha256:e09c3e2a3585def05d2df2b4cf20f14507e226353037c849880f052ba4b79c5d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.6 MB (165559629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e44dc995e2ffda45a603609157c0d760c4197795cbf6b05bed904e22b4ff52a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 07 Feb 2023 11:05:29 GMT
RUN Apply image 10.0.20348.1547
# Wed, 15 Feb 2023 23:34:03 GMT
SHELL [cmd /s /c]
# Wed, 15 Feb 2023 23:37:44 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Wed, 15 Feb 2023 23:37:45 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 15 Feb 2023 23:37:46 GMT
USER ContainerAdministrator
# Wed, 15 Feb 2023 23:37:57 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 15 Feb 2023 23:37:58 GMT
USER ContainerUser
# Wed, 15 Feb 2023 23:39:22 GMT
COPY dir:bfcbd3aaadac52e2fbf5597edb59a69874950e88ce16232f7581c0ac600a935c in C:\openjdk-17 
# Wed, 15 Feb 2023 23:39:41 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:2e8a1636f1721beefd71f8e0c7176faabfe00d7503a69e909468fd63ac3a4992`  
		Last Modified: Thu, 16 Feb 2023 00:30:27 GMT  
		Size: 122.1 MB (122119166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f21b41cddbbbe3e6e7b8691f9cfc05eac50290ddadabfd44482b251564c6481`  
		Last Modified: Thu, 16 Feb 2023 07:21:04 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3658899f6e99d81760c3887ea095c78d012196fe47f4863285f3999bb6612e17`  
		Last Modified: Thu, 16 Feb 2023 07:22:48 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1331eed267029729290625bbd454aa75a1c022972206a9518b0c0282d64d2bca`  
		Last Modified: Thu, 16 Feb 2023 07:22:48 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6c23ca29360229721d35d3d391409b7abfc544d9d0eb97a96df2cca2816617`  
		Last Modified: Thu, 16 Feb 2023 07:22:48 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0078d6c15b13291e0ab1bb1e6544111c047874f37b3c00be791026226af5075`  
		Last Modified: Thu, 16 Feb 2023 07:22:46 GMT  
		Size: 85.6 KB (85578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a20db78bb523ad6d898d6509eede0ad5ff051b28a768ac731bc21b2e2c03fc5f`  
		Last Modified: Thu, 16 Feb 2023 07:22:46 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721e55f8cfe8a7c08c417ae302554eca115e62075065ea494b421bc6f62852d3`  
		Last Modified: Thu, 16 Feb 2023 07:23:35 GMT  
		Size: 43.3 MB (43287527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443edbf80faaf617fb0cb0fdc2460bfba8afcae4fac386ad50b867348d0d131a`  
		Last Modified: Thu, 16 Feb 2023 07:23:24 GMT  
		Size: 62.0 KB (62047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
