## `eclipse-temurin:17-jre-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:f87de364067f0543d1a334c83ca6e8ee5c2c9177de5af2b3a4e7c780fda2283c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1668; amd64
	-	windows version 10.0.17763.4252; amd64

### `eclipse-temurin:17-jre-nanoserver` - windows version 10.0.20348.1668; amd64

```console
$ docker pull eclipse-temurin@sha256:a54eb3336579405a0c71c5463b9e1b7786c2c4057749178e5e0387f0b799e698
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.8 MB (165806595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:019d086b1d67e27985e7b5f9487c15f825fbcf0b415ac7ec835f30e16555076a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:16 GMT
RUN Apply image 10.0.20348.1668
# Wed, 12 Apr 2023 01:42:21 GMT
SHELL [cmd /s /c]
# Wed, 26 Apr 2023 19:54:42 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 26 Apr 2023 19:54:42 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 26 Apr 2023 19:54:43 GMT
USER ContainerAdministrator
# Wed, 26 Apr 2023 19:54:52 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 26 Apr 2023 19:54:53 GMT
USER ContainerUser
# Wed, 26 Apr 2023 19:55:33 GMT
COPY dir:8912d07424b5206284ef3b7586d69c3f366b527bba3d6f334194ae58c2152641 in C:\openjdk-17 
# Wed, 26 Apr 2023 19:55:45 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:e06b772d586b58466a653b72002aee7c59496110e9ae402ff58f026e44452506`  
		Last Modified: Wed, 12 Apr 2023 02:34:14 GMT  
		Size: 122.3 MB (122328782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8058ec80ac2516d001291dea383d4abfa22416397a4c869e6fd79c0d4b64565f`  
		Last Modified: Wed, 12 Apr 2023 09:45:40 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c34e9a0ac29e9b495785851009aecac2384be077142f5473c0b0953c4a8c9db`  
		Last Modified: Wed, 26 Apr 2023 20:11:02 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09977fadc4c78d42c9f86687814da32e098de1f026b455876766527eead98a7a`  
		Last Modified: Wed, 26 Apr 2023 20:11:02 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77255777319739b0433d525fc1ad4d4ec38d9ae4a8ab4caa2abb5af02c123a80`  
		Last Modified: Wed, 26 Apr 2023 20:11:01 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8e543926a3b03fff632c6696b921848562af2e600ddafd31a9b2bcf918b803`  
		Last Modified: Wed, 26 Apr 2023 20:11:00 GMT  
		Size: 84.4 KB (84374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4c401511e4d0c7d5a53409a95fd8da066fec7e6622e32f574b8012319841a5`  
		Last Modified: Wed, 26 Apr 2023 20:11:00 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68e78841cc28bf6b9617501374f5f5ff547b180c149d5d45d29299ae0410955`  
		Last Modified: Wed, 26 Apr 2023 20:11:38 GMT  
		Size: 43.3 MB (43326163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a0cb620119f9a4c1173079af7581b220e7b0d21da9c02c5d2aef2ce116d136`  
		Last Modified: Wed, 26 Apr 2023 20:11:29 GMT  
		Size: 62.0 KB (61974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:17-jre-nanoserver` - windows version 10.0.17763.4252; amd64

```console
$ docker pull eclipse-temurin@sha256:901afe3140ff2746040bcab701733bb76260191f12b1353e0f0d335250b90fe0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.2 MB (153247849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37ce8650ab4c254a47363ac7c8016ebaccdbe625a74da2f4907801f15f9a73d9`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Tue, 11 Apr 2023 23:45:41 GMT
SHELL [cmd /s /c]
# Wed, 26 Apr 2023 19:38:03 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 26 Apr 2023 19:38:04 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 26 Apr 2023 19:38:05 GMT
USER ContainerAdministrator
# Wed, 26 Apr 2023 19:38:13 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 26 Apr 2023 19:38:14 GMT
USER ContainerUser
# Wed, 26 Apr 2023 19:42:41 GMT
COPY dir:8912d07424b5206284ef3b7586d69c3f366b527bba3d6f334194ae58c2152641 in C:\openjdk-17 
# Wed, 26 Apr 2023 19:42:52 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
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
	-	`sha256:17a1ec02fa1d12354c3753a642e82d439a151eb4c0fe52d0a95babfcbf24a47a`  
		Last Modified: Wed, 26 Apr 2023 20:05:27 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e86c12c67ae63b7b121d66001fcb205fd8bd4641fdebd02717a7b30049358d61`  
		Last Modified: Wed, 26 Apr 2023 20:05:27 GMT  
		Size: 1.0 KB (1029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85d77dd737462ca8131dfd15ac168bc3279cafd6e812fbe09771dc09b57e216`  
		Last Modified: Wed, 26 Apr 2023 20:05:27 GMT  
		Size: 1.1 KB (1082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08ae7a2ea51900ae87c5fcde372760769e9a78a91e3cf0edb6a8c8df38a68d0`  
		Last Modified: Wed, 26 Apr 2023 20:05:25 GMT  
		Size: 74.2 KB (74159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050ed453bb1642ab3df2bb207b1b589342eabede15dc9bf2975f09eb04646ab4`  
		Last Modified: Wed, 26 Apr 2023 20:05:25 GMT  
		Size: 1.0 KB (1029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b66526444dcbb2e3c38f24e5ae4807c7f2675ecc279eb033d80a757981bc9de`  
		Last Modified: Wed, 26 Apr 2023 20:06:40 GMT  
		Size: 43.3 MB (43328529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d749afdfd5a5c91caeaea0d46c2022953cff59708a9eea268a13ebd28b1ae6d7`  
		Last Modified: Wed, 26 Apr 2023 20:06:32 GMT  
		Size: 3.1 MB (3050878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
