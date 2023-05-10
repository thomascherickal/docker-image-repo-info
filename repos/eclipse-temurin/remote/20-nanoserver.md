## `eclipse-temurin:20-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:ba824160d936719f662bf9e68ddb0dd6cd6a26251bf4f5b8d5013271264245b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1726; amd64
	-	windows version 10.0.17763.4377; amd64

### `eclipse-temurin:20-nanoserver` - windows version 10.0.20348.1726; amd64

```console
$ docker pull eclipse-temurin@sha256:b9ee0b6d8bb85b6dfcc1962e9d06cd728610ab40eedb3faa30bb51f1640cd966
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.4 MB (315432775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:176226a4dc8658444e180a2d3de155cb93bf0613cff18f080060447fb2a7418b`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 05 May 2023 12:52:54 GMT
RUN Apply image 10.0.20348.1726
# Wed, 10 May 2023 01:13:54 GMT
SHELL [cmd /s /c]
# Wed, 10 May 2023 01:17:33 GMT
ENV JAVA_VERSION=jdk-20.0.1+9
# Wed, 10 May 2023 01:17:34 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 10 May 2023 01:17:34 GMT
USER ContainerAdministrator
# Wed, 10 May 2023 01:17:43 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 10 May 2023 01:17:44 GMT
USER ContainerUser
# Wed, 10 May 2023 01:17:59 GMT
COPY dir:f42e28541c92f419d16f8f9260ba58e12cc63ca253028a61fc42e8a28f91cd69 in C:\openjdk-20 
# Wed, 10 May 2023 01:18:13 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 10 May 2023 01:18:14 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:7d382efe6974b94c05000b6a95c1fd28e1b8bb3e81cc4592b2aa1cc46b90192c`  
		Last Modified: Wed, 10 May 2023 01:48:23 GMT  
		Size: 120.0 MB (120001338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cfc306feea2a215b4a83a66480231042a4bdc8001d07d634086f52f1f5ab3c`  
		Last Modified: Wed, 10 May 2023 07:04:09 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:102b5285ff20b5da43698a254b019623d13fa0fff343e58f02364a7fade0f9a9`  
		Last Modified: Wed, 10 May 2023 07:06:14 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed92b05a447b82514f3ed09c8800f00450d6dfaf4a834d5c4e89a7721c06362`  
		Last Modified: Wed, 10 May 2023 07:06:14 GMT  
		Size: 1.1 KB (1064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:263c8320754a70ba87c2bfe5f942d9c40c5ba1ee480bbae87511d66fe8e18bbd`  
		Last Modified: Wed, 10 May 2023 07:06:14 GMT  
		Size: 1.1 KB (1082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c78515dd5692679ff78e48ff2ec16e74323946877ef490c6f5deaa177d7617ac`  
		Last Modified: Wed, 10 May 2023 07:06:12 GMT  
		Size: 87.3 KB (87340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:789563d9e96a6480dbdb98188690acdd4debcf1e4f88704749b2dca25f108111`  
		Last Modified: Wed, 10 May 2023 07:06:12 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7270b423dab2f7e86cbe277fdbcf9ad93d1e727a5aa5540959d5b6e2aa358952`  
		Last Modified: Wed, 10 May 2023 07:06:31 GMT  
		Size: 195.3 MB (195277033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b160eda48493090f780728650a9270b3ac3c39d790c40c43f079420d136b06`  
		Last Modified: Wed, 10 May 2023 07:06:12 GMT  
		Size: 60.8 KB (60792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ca9c7e79d50c3443432bbb6fc12f02d2e09e97d0a37aeabfb38104791d27533`  
		Last Modified: Wed, 10 May 2023 07:06:12 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:20-nanoserver` - windows version 10.0.17763.4377; amd64

```console
$ docker pull eclipse-temurin@sha256:63fae7247a7186e532de84a5a95f15f5f16fcc4443b06fffaca09e31ac8ac689
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.5 MB (303510627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41b7c219436ab2399573ab39897e26d5eba8cc1d0054992cbe090d5a4a53e884`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 05 May 2023 11:29:01 GMT
RUN Apply image 10.0.17763.4377
# Wed, 10 May 2023 00:40:01 GMT
SHELL [cmd /s /c]
# Wed, 10 May 2023 01:08:43 GMT
ENV JAVA_VERSION=jdk-20.0.1+9
# Wed, 10 May 2023 01:08:44 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 10 May 2023 01:08:44 GMT
USER ContainerAdministrator
# Wed, 10 May 2023 01:08:56 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 10 May 2023 01:08:57 GMT
USER ContainerUser
# Wed, 10 May 2023 01:09:12 GMT
COPY dir:f42e28541c92f419d16f8f9260ba58e12cc63ca253028a61fc42e8a28f91cd69 in C:\openjdk-20 
# Wed, 10 May 2023 01:09:29 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 10 May 2023 01:09:30 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:f7885e3a2dfeae5eea125d00da688c29930a05e4d904884fe43e093ce6223664`  
		Last Modified: Wed, 10 May 2023 01:49:01 GMT  
		Size: 104.4 MB (104383998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b79dd15c5dd82bc10521b9a4e49241f70088bc6edbb286f90be198abea55e23`  
		Last Modified: Wed, 10 May 2023 03:01:27 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebeed88a3c3c66be9d16b0f957117b6a05a44f2ac948dd4aca0f43c68d160623`  
		Last Modified: Wed, 10 May 2023 07:02:44 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25505a5fb14945526218e6746c3daf3a5d7871920141d83cd21678564081efd`  
		Last Modified: Wed, 10 May 2023 07:02:44 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4ed7459bd32a803e36cfed0d698f9a4adffaee96bd076051f2126e9c2a3f0c`  
		Last Modified: Wed, 10 May 2023 07:02:45 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f804cc4402ea0e2cf02b8eabc30456d191d800ec769ebf94865dcd968057ca`  
		Last Modified: Wed, 10 May 2023 07:02:43 GMT  
		Size: 66.7 KB (66721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef79afd7f3bdb4142c1af32cbff138ac87b254f0d67e10185503043390adcbb4`  
		Last Modified: Wed, 10 May 2023 07:02:43 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd81aefbafb5637044ca05e5349f5f3cb0d9400761a76d6d1b0602301e1ae51`  
		Last Modified: Wed, 10 May 2023 07:03:01 GMT  
		Size: 195.3 MB (195278085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b03ebd7ae8ae4945860c5ba0ee2ba28dae1d39d38ba018c9daf1fa9c9aa5a1e`  
		Last Modified: Wed, 10 May 2023 07:02:44 GMT  
		Size: 3.8 MB (3774818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3280576ae4d055c84491d3aace0b71bc572d9e92ccdd15fc913104a98d989441`  
		Last Modified: Wed, 10 May 2023 07:02:43 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
