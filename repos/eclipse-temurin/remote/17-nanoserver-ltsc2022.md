## `eclipse-temurin:17-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:34659595fd6850edb2683af01860768974fb9aa0f3cb05aa11d299908ac24490
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.587; amd64

### `eclipse-temurin:17-nanoserver-ltsc2022` - windows version 10.0.20348.587; amd64

```console
$ docker pull eclipse-temurin@sha256:5d1d5a04a97a846ed97fdb6489574866cb905492115e3dd69cae1b63b6ea65dc
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.7 MB (302653527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:216add0dce60a84f2e510eb90426c03578038099b7eda211224ddfa3a3f259b2`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 03 Mar 2022 04:50:34 GMT
RUN Apply image ltsc2022-amd64
# Tue, 08 Mar 2022 22:26:00 GMT
SHELL [cmd /s /c]
# Tue, 08 Mar 2022 22:29:10 GMT
ENV JAVA_VERSION=jdk-17.0.2+8
# Tue, 08 Mar 2022 22:29:10 GMT
ENV JAVA_HOME=C:\openjdk-17
# Tue, 08 Mar 2022 22:29:11 GMT
USER ContainerAdministrator
# Tue, 08 Mar 2022 22:29:22 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Tue, 08 Mar 2022 22:29:23 GMT
USER ContainerUser
# Tue, 08 Mar 2022 22:29:37 GMT
COPY dir:af72ba1102e9cda7f5ea9974b0cafbe96b2f97690adb0743202a1c732a987a84 in C:\openjdk-17 
# Tue, 08 Mar 2022 22:29:57 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 08 Mar 2022 22:29:58 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:dad81795ce109a7e20ebf80ad31925797ed97f9ba2a559f13f96ce3be5ea712b`  
		Size: 117.5 MB (117485491 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ad17ae3a2fc5cdf554f0d828bd6d04e79f37ae3dd800a44c8a3a1892a57b75c3`  
		Last Modified: Tue, 08 Mar 2022 22:57:38 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a2d191ed154acbc5f87c0c16303ef84a425ae3b20ff0ef131d9d1f6ea1e0e9`  
		Last Modified: Tue, 08 Mar 2022 23:03:22 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ef17868c695af7053447548c30b3befe6c902692291edd2706a6275a89631c`  
		Last Modified: Tue, 08 Mar 2022 23:03:22 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8749dcdd44bfcf8927ece700e5ec010daad5c3daff63f5f9e993beba36fd11`  
		Last Modified: Tue, 08 Mar 2022 23:03:22 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc3a78d8d11295a20622c3299b08f453bf1417b8cfca0f7d3f4a12ee4b482fe`  
		Last Modified: Tue, 08 Mar 2022 23:03:20 GMT  
		Size: 85.2 KB (85158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c5f95c2833f07d793777fbd4d6bcde63ff4fc108458e4531b21c3880b4fd2e`  
		Last Modified: Tue, 08 Mar 2022 23:03:20 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2193182604e022490e8c2fe6aeef5a51f772169c748dbe45c275e5832fbea6be`  
		Last Modified: Tue, 08 Mar 2022 23:06:56 GMT  
		Size: 185.0 MB (185014208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82963cf92683d3bec541e247c1797f895b1e1304f4377a4863fe52a710e4be0`  
		Last Modified: Tue, 08 Mar 2022 23:03:20 GMT  
		Size: 61.7 KB (61689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4acd104b3fc36a35a6508934bf1f843a0adb6b8b2d879429a64ede5c92e888ce`  
		Last Modified: Tue, 08 Mar 2022 23:03:20 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
