## `eclipse-temurin:17-jdk-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:037c2053904b303690a2450b2a1250baa3b5d5b980a2b78caec564408d2fc023
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.2031; amd64
	-	windows version 10.0.17763.4974; amd64

### `eclipse-temurin:17-jdk-nanoserver` - windows version 10.0.20348.2031; amd64

```console
$ docker pull eclipse-temurin@sha256:17add7b45531ec140f99736f7622bb16ef5b842293f97594a098b94282d5f015
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.5 MB (306482538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:432ff477d3048dabdd4edca44177ffc18f8adaa1b5245dd4c3c9e9d0f033495f`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 06 Oct 2023 21:30:39 GMT
RUN Apply image 10.0.20348.2031
# Wed, 11 Oct 2023 02:14:39 GMT
SHELL [cmd /s /c]
# Wed, 11 Oct 2023 02:16:57 GMT
ENV JAVA_VERSION=jdk-17.0.8.1+1
# Wed, 11 Oct 2023 02:16:57 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 11 Oct 2023 02:16:58 GMT
USER ContainerAdministrator
# Wed, 11 Oct 2023 02:17:08 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 11 Oct 2023 02:17:09 GMT
USER ContainerUser
# Wed, 11 Oct 2023 02:17:22 GMT
COPY dir:87d4868aeffb4665dc24a8514128e3f1a9351c7c90320c533fd29622fc9de6e2 in C:\openjdk-17 
# Wed, 11 Oct 2023 02:17:33 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 11 Oct 2023 02:17:34 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:fff54800e03713ba81736f43d985319592fc643a1a32b62dbd5c0ec36549de00`  
		Last Modified: Tue, 10 Oct 2023 17:30:43 GMT  
		Size: 120.6 MB (120604344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142fccf33f15e2c503ce4023e2e496d7a99bd036e8b83264772e9dab49c325b3`  
		Last Modified: Wed, 11 Oct 2023 07:29:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a659a6819c82d820046e21dc8f4b451012170ce85c646026870c3d99697e82`  
		Last Modified: Wed, 11 Oct 2023 07:30:59 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f37f39162b0c25f89383c864eff970e2b4d474348c83f10f297506e925beeaa`  
		Last Modified: Wed, 11 Oct 2023 07:30:59 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcb33551667e9e57741cdfc91f6b464adf39fa78ce6d380b810e0c61253726e`  
		Last Modified: Wed, 11 Oct 2023 07:30:59 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d5b0fac9bcddc489ced725a45a3f43c3f60cae734c5b82b37fbc9ed799aded`  
		Last Modified: Wed, 11 Oct 2023 07:30:57 GMT  
		Size: 87.9 KB (87919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4834e380ffecef09c287647d524c63045c541ae357d316f993087a6e72a88af`  
		Last Modified: Wed, 11 Oct 2023 07:30:57 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48acdc32c8bf39ecfc807a3b8bc481b1f21488e4bbdbf8683b9bf1631f998bab`  
		Last Modified: Wed, 11 Oct 2023 07:31:17 GMT  
		Size: 185.7 MB (185725966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae6ca288fdb7a2a231a80851d6ed8eeed365dfac317f37a2ab3ec00427a5a940`  
		Last Modified: Wed, 11 Oct 2023 07:30:57 GMT  
		Size: 57.4 KB (57363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6850ba1ac3ea06bfd3a8b4a7e047cb797000e822bacf5f563b16f2628c9747`  
		Last Modified: Wed, 11 Oct 2023 07:30:57 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:17-jdk-nanoserver` - windows version 10.0.17763.4974; amd64

```console
$ docker pull eclipse-temurin@sha256:06866bd3b45fdf0dc15b16cb2daacc43f85d9cc39b565f344786b4f2aad35963
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.9 MB (293902588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30e0d3e73b0ae94d4162e5f26d0a2ec768e66e22349777accb660d4a56d7b3d3`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 01:39:37 GMT
SHELL [cmd /s /c]
# Wed, 11 Oct 2023 01:59:11 GMT
ENV JAVA_VERSION=jdk-17.0.8.1+1
# Wed, 11 Oct 2023 01:59:11 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 11 Oct 2023 01:59:12 GMT
USER ContainerAdministrator
# Wed, 11 Oct 2023 01:59:20 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 11 Oct 2023 01:59:21 GMT
USER ContainerUser
# Wed, 11 Oct 2023 01:59:33 GMT
COPY dir:87d4868aeffb4665dc24a8514128e3f1a9351c7c90320c533fd29622fc9de6e2 in C:\openjdk-17 
# Wed, 11 Oct 2023 01:59:44 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 11 Oct 2023 01:59:45 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5f8edc2588edb9971a52d53cd4265062614ebb25e94063a4d235376797b0e57a`  
		Last Modified: Tue, 10 Oct 2023 17:24:08 GMT  
		Size: 104.5 MB (104464580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c11581d9ee9ea19d58c6cbb415dd809a51b56502169a7a5b301da76d79f63b`  
		Last Modified: Wed, 11 Oct 2023 03:57:05 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:910f6f917f2cdf2e22c1ef319d158e41cdd745eb4a32c6b0d2aa0d3bdbed0fb1`  
		Last Modified: Wed, 11 Oct 2023 07:25:30 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363c054ef4256dc6307777435e2ed3b7305de2592f0efe9099b44656f2989a14`  
		Last Modified: Wed, 11 Oct 2023 07:25:29 GMT  
		Size: 1.1 KB (1065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cca7cabc17de1b2985aec2e23123bf7c78f0338feffc73de14e1a31e586e477`  
		Last Modified: Wed, 11 Oct 2023 07:25:29 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d05a4a445514fd6e92563a39b4ea5ec855ce3d759b67145b2425b96cb1179f`  
		Last Modified: Wed, 11 Oct 2023 07:25:27 GMT  
		Size: 71.2 KB (71182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf96c564af030f823869568c5f79ec57ac99a32a159376d4af050e2069973ea`  
		Last Modified: Wed, 11 Oct 2023 07:25:27 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ae9cdb2aa55e3a3ecaa19179f3214a66ce4783e9accf80d6e08720261e6cdb`  
		Last Modified: Wed, 11 Oct 2023 07:25:46 GMT  
		Size: 185.7 MB (185726951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a00045a364948b07d3bb8040785438162a24defa21b4b17f37629fa83676b1`  
		Last Modified: Wed, 11 Oct 2023 07:25:28 GMT  
		Size: 3.6 MB (3633538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbaf220abc6714c3614e8d4c771e3fb569cf321e248037ddca7d3afa26ae84ca`  
		Last Modified: Wed, 11 Oct 2023 07:25:27 GMT  
		Size: 1.0 KB (1029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
