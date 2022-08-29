## `eclipse-temurin:18-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:a9293a216f4e12e05467b2e7b21c36ca07f1ed862ba6471bae348348218289e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.887; amd64
	-	windows version 10.0.17763.3287; amd64

### `eclipse-temurin:18-nanoserver` - windows version 10.0.20348.887; amd64

```console
$ docker pull eclipse-temurin@sha256:42f808be2c38b65af6a0cc54a6fad7b10ac349c1abc39017a442c8699722ca37
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.8 MB (304770882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28a052f5ee7f80bc28e4b69f21efe86f4f5c138d9706476717aeceb99c8527c8`
-	Default Command: `["jshell"]`
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
# Mon, 29 Aug 2022 18:30:18 GMT
COPY dir:ae9d728ada666b27b908f8727aedf35273804bd829b96771abae3f99230f2142 in C:\openjdk-18 
# Mon, 29 Aug 2022 18:30:39 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Mon, 29 Aug 2022 18:30:41 GMT
CMD ["jshell"]
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
	-	`sha256:d598a60dcbbe4c9a861a8e4665e38fabcdd8d5e5a036a3b4e7cbda1d2b0e4470`  
		Last Modified: Mon, 29 Aug 2022 18:37:46 GMT  
		Size: 186.5 MB (186536865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe92df993132858c6f4a7ee27cc5cf6e88bf9e4db3c130ed86aea50f26289a2`  
		Last Modified: Mon, 29 Aug 2022 18:37:28 GMT  
		Size: 61.4 KB (61416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023405962c31144b90cf386bb9860fdfa1c34921f8016a4af0ca99b3ac3ba7e9`  
		Last Modified: Mon, 29 Aug 2022 18:37:28 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:18-nanoserver` - windows version 10.0.17763.3287; amd64

```console
$ docker pull eclipse-temurin@sha256:7f2d8d91921acf44c6465b4427c42158ecd22295d032ef0fd6b03a03d55193b8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.4 MB (293401056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a37aa6506efbde9820c8bbf49b1780d2f94510820db0f80fcb6a058879bc5af1`
-	Default Command: `["jshell"]`
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
# Mon, 29 Aug 2022 18:24:16 GMT
COPY dir:ae9d728ada666b27b908f8727aedf35273804bd829b96771abae3f99230f2142 in C:\openjdk-18 
# Mon, 29 Aug 2022 18:24:37 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Mon, 29 Aug 2022 18:24:39 GMT
CMD ["jshell"]
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
	-	`sha256:1bb951e66d1028712608596c4dba0123b6449ef788c4d7451a81eb299be02421`  
		Last Modified: Mon, 29 Aug 2022 18:36:09 GMT  
		Size: 186.6 MB (186551569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e3c5ee49f9a5e35eb53ee4d9cfd17851da73597a9c19ea23c4ead16fbc4c83`  
		Last Modified: Mon, 29 Aug 2022 18:35:52 GMT  
		Size: 3.6 MB (3567581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f1eca4649f841c1fa5c3327f2c41fd0a98c5aafb6dda3581a005b0ca988de8`  
		Last Modified: Mon, 29 Aug 2022 18:35:51 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
