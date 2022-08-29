## `eclipse-temurin:18-jre-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:4b1907e1e4b554b857959850c28b237179a627994c5ae44e6ee89132a9640676
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.887; amd64
	-	windows version 10.0.17763.3287; amd64

### `eclipse-temurin:18-jre-nanoserver` - windows version 10.0.20348.887; amd64

```console
$ docker pull eclipse-temurin@sha256:b1e65b42a34d9e45288867027869e2a216750d081652751fa909d3dd21810098
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.4 MB (161370915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c606dbf3a2c407e57ecbb6e7a217815a6a14fd0b8e0af97fb82e6cbede793f5f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 06 Aug 2022 18:05:23 GMT
RUN Apply image 10.0.20348.887
# Wed, 10 Aug 2022 16:28:17 GMT
SHELL [cmd /s /c]
# Mon, 29 Aug 2022 18:29:40 GMT
ENV JAVA_VERSION=jdk-18.0.2.1+1
# Mon, 29 Aug 2022 18:29:42 GMT
ENV JAVA_HOME=C:\openjdk-18
# Mon, 29 Aug 2022 18:29:44 GMT
USER ContainerAdministrator
# Mon, 29 Aug 2022 18:29:59 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Mon, 29 Aug 2022 18:30:01 GMT
USER ContainerUser
# Mon, 29 Aug 2022 18:31:05 GMT
COPY dir:0f122a29933687aee1aeb1ed0bbcab77514458b9f4eb8e7fa2df7c081ea3d7bd in C:\openjdk-18 
# Mon, 29 Aug 2022 18:31:19 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:2ebf439f800cd4c1fccaf4a0545e6bff60caa5141295c8ab81f6c525073c423d`  
		Size: 118.1 MB (118088450 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5f1e06146ab0490d235fe89786637467a4b71853ee428e8740ea6efbc536c47c`  
		Last Modified: Wed, 10 Aug 2022 16:48:40 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6872ddd0a0bf2c680b4627d709b696212df1abf48fc184eceec0d0f12f44f23c`  
		Last Modified: Mon, 29 Aug 2022 18:37:31 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1df8b77de69b55d37ed5a721b11b15808786f88eba2cdd8e8cfea32943d9ad`  
		Last Modified: Mon, 29 Aug 2022 18:37:31 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370f713fbfd7c5165e0b58aea88ca2711dadfd2df3017a18a77180d449315f99`  
		Last Modified: Mon, 29 Aug 2022 18:37:30 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882c4ac003caa6b022c9e778cf3359512b1f882387af9fec81c42d7fdfabbfbd`  
		Last Modified: Mon, 29 Aug 2022 18:37:28 GMT  
		Size: 77.2 KB (77204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ed4eb12e1e24ed33ab5a14a437b6f76c129208fe10ef0530d73b2f551ce7ee`  
		Last Modified: Mon, 29 Aug 2022 18:37:28 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdfc3d66dac6a39fc1166a0ba29d78c69c10d3e85680449a6510de5c72d3dc4a`  
		Last Modified: Mon, 29 Aug 2022 18:38:06 GMT  
		Size: 43.1 MB (43138174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476dc75ed56f71338a6cf5b24dc7fbaba65343a792fe42f9e2d31121b8d2d48e`  
		Last Modified: Mon, 29 Aug 2022 18:37:59 GMT  
		Size: 61.3 KB (61321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:18-jre-nanoserver` - windows version 10.0.17763.3287; amd64

```console
$ docker pull eclipse-temurin@sha256:143f3f0cca5efd91a1fbeb7f5f4b612cd94574bf686c2a1b2ddf2dc931788139
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.4 MB (149362454 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56f98d1f1a55e13d40b8a96d383b1f9b06e71963c9d4ec0aba3258d3ba824773`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 06 Aug 2022 18:08:38 GMT
RUN Apply image 10.0.17763.3287
# Wed, 10 Aug 2022 15:57:07 GMT
SHELL [cmd /s /c]
# Mon, 29 Aug 2022 18:23:38 GMT
ENV JAVA_VERSION=jdk-18.0.2.1+1
# Mon, 29 Aug 2022 18:23:40 GMT
ENV JAVA_HOME=C:\openjdk-18
# Mon, 29 Aug 2022 18:23:42 GMT
USER ContainerAdministrator
# Mon, 29 Aug 2022 18:23:57 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Mon, 29 Aug 2022 18:23:59 GMT
USER ContainerUser
# Mon, 29 Aug 2022 18:28:41 GMT
COPY dir:0f122a29933687aee1aeb1ed0bbcab77514458b9f4eb8e7fa2df7c081ea3d7bd in C:\openjdk-18 
# Mon, 29 Aug 2022 18:28:56 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:5c9d6483dab113d2d9b50fdf3156622aa2ec3d6faaed5664d15a5568032d1714`  
		Size: 103.2 MB (103204200 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0f4438539876006761cb687527bd8cb94cc7a273cf8bb47563981044f2e1771e`  
		Last Modified: Wed, 10 Aug 2022 16:38:40 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079c8019b8d860add7e469efe084e361401eccb80eea879d6cbe4aaf0739d422`  
		Last Modified: Mon, 29 Aug 2022 18:35:54 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff09b635a581659c5e7a0c8e3757bf70e464f2ccadd4cfca1d216e1f9a62bc8`  
		Last Modified: Mon, 29 Aug 2022 18:35:54 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c09109e3ba671de263b5e0254bf16697599a7f4cff277eac6b17b536d8da26`  
		Last Modified: Mon, 29 Aug 2022 18:35:54 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52d5855590b900da119bf781ec14b2275d8ad785c2c621f2ace60dac79740a34`  
		Last Modified: Mon, 29 Aug 2022 18:35:51 GMT  
		Size: 70.8 KB (70812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd9b924fc322681a5fbbcc5b5c5f0d6108d37616bacd0d613e1e9fe685e41c52`  
		Last Modified: Mon, 29 Aug 2022 18:35:51 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01601f091dc7483a14152d559c249e6c83432f035e7d97eea906253b04c7a282`  
		Last Modified: Mon, 29 Aug 2022 18:37:12 GMT  
		Size: 43.1 MB (43138172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9d68ced9dabd223d70d9bc2834643947ec4e398feefe6e2e7e24f44bea4ef4`  
		Last Modified: Mon, 29 Aug 2022 18:37:05 GMT  
		Size: 2.9 MB (2943548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
