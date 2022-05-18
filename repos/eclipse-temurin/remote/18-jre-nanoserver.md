## `eclipse-temurin:18-jre-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:2247ec7bf4396524a202718f11d1a72c97a6c9d07bd323eec8e3f2242544a315
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.707; amd64
	-	windows version 10.0.17763.2928; amd64

### `eclipse-temurin:18-jre-nanoserver` - windows version 10.0.20348.707; amd64

```console
$ docker pull eclipse-temurin@sha256:9c498cf150ed270f26ad25e7fba9c59e065173996e8a23fce767111d1c3aeb25
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.9 MB (160875748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15319e45845a8ae279aff30fc40f145ef8c6a3007cbb1265c6b9f488c1cdd140`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 05 May 2022 02:37:33 GMT
RUN Apply image 10.0.20348.707
# Wed, 11 May 2022 15:21:54 GMT
SHELL [cmd /s /c]
# Wed, 11 May 2022 15:26:29 GMT
ENV JAVA_VERSION=jdk-18.0.1+10
# Wed, 11 May 2022 15:26:30 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 11 May 2022 15:26:30 GMT
USER ContainerAdministrator
# Wed, 11 May 2022 15:26:41 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 11 May 2022 15:26:42 GMT
USER ContainerUser
# Wed, 11 May 2022 15:27:30 GMT
COPY dir:ba165d8363f6d3c715a5361167e7667ee35da551a187f89de48613c79c89ce98 in C:\openjdk-18 
# Wed, 11 May 2022 15:27:49 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:2c74f0842c5a8e9b80b9e2cf64e1ab10a6fa67951f28cff5fee060b88128564c`  
		Size: 117.7 MB (117687017 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c783ef8875d74b7e18cf09914325e131a525d4678bc9b243734768fdbcde89a2`  
		Last Modified: Wed, 18 May 2022 13:44:02 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d136dfaf5ae7a851d8ea1efa3640d91012139c0f92483b78c3a9be76f27d6fdd`  
		Last Modified: Wed, 18 May 2022 13:54:05 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0470945a9c0833003c1fc65d3ad2497db1049955e680861d181d817082c8491f`  
		Last Modified: Wed, 18 May 2022 13:54:05 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237cc5aee4d5732a84f29974bd6a67d4505998acf73f70352dd540353981926d`  
		Last Modified: Wed, 18 May 2022 13:54:05 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb2b36d85adcba260435f5c6f962c7ccdbba274a95df2318ef4a7bc6dbf4dcd`  
		Last Modified: Wed, 18 May 2022 13:54:03 GMT  
		Size: 76.1 KB (76145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46ca06f941a094e65b95e7e8c2bd2d3775c06217ef567cec0555dcdb1096740`  
		Last Modified: Wed, 18 May 2022 13:54:03 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e368920ad76c269b3bf5de658dd6358fff1f468eff09502dbf748434978bee`  
		Last Modified: Wed, 18 May 2022 13:55:21 GMT  
		Size: 43.0 MB (43047347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5903a3a249e18e14443b2a8a5399d4578112fc0e4581f4cbf997afe20876a6d6`  
		Last Modified: Wed, 18 May 2022 13:54:34 GMT  
		Size: 59.5 KB (59505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:18-jre-nanoserver` - windows version 10.0.17763.2928; amd64

```console
$ docker pull eclipse-temurin@sha256:76ca994de79693d7de1893a7f41841d443b92f8fe5b0fb2a13eb70f077b28cee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.2 MB (149157862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7726bf2cfdada5c676dff6207781e1a50518b30799f8bf6315d404747a45bae4`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 05 May 2022 16:42:43 GMT
RUN Apply image 10.0.17763.2928
# Wed, 11 May 2022 14:49:49 GMT
SHELL [cmd /s /c]
# Wed, 11 May 2022 15:17:11 GMT
ENV JAVA_VERSION=jdk-18.0.1+10
# Wed, 11 May 2022 15:17:11 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 11 May 2022 15:17:12 GMT
USER ContainerAdministrator
# Wed, 11 May 2022 15:17:21 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 11 May 2022 15:17:22 GMT
USER ContainerUser
# Wed, 11 May 2022 15:21:33 GMT
COPY dir:ba165d8363f6d3c715a5361167e7667ee35da551a187f89de48613c79c89ce98 in C:\openjdk-18 
# Wed, 11 May 2022 15:21:45 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:6626f490e738e10ea5e31ff2643e3a8c372e076d9030c77fac37537dbf12b73c`  
		Size: 103.1 MB (103133833 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5592374182790eb41396d922d16be86f39a125562f29ea3ed221a94aeec2af45`  
		Last Modified: Wed, 11 May 2022 16:00:35 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932168d2a841e72a2f7aa4e6e4ceb658cc49fb857d20f25b6df0a1ba3ae9ada4`  
		Last Modified: Wed, 18 May 2022 13:40:43 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23a48d381b79496bd03d17f3dc7d85911ca74ec0f4934915a4acaa24cf1001d`  
		Last Modified: Wed, 18 May 2022 13:40:43 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8884618775190e454a9daac184259eca381568414ee0755e99c57f42fe4a95`  
		Last Modified: Wed, 18 May 2022 13:40:43 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c902b1c5d9ecd421c4cfe2b1e768a78722666b89f6d49d41c8a2b4fda7af9e`  
		Last Modified: Wed, 18 May 2022 13:40:40 GMT  
		Size: 72.0 KB (71993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295c01d0a06b53e0ad6831f9c1b9d6f400122229fa154dce8e9eaf6cf4f3a96d`  
		Last Modified: Wed, 18 May 2022 13:40:41 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad38478fd8c8217702e59201817eae697d3b5d9deda5fbcb1718e1d9641f71e4`  
		Last Modified: Wed, 18 May 2022 13:43:50 GMT  
		Size: 43.0 MB (43038126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fd92fcb1ac14c1198c942509e1a01a3fa3d4a8f2726f7989518234181a7b140`  
		Last Modified: Wed, 18 May 2022 13:43:05 GMT  
		Size: 2.9 MB (2908145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
