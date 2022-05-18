## `eclipse-temurin:8u332-b09-jre-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:a2dfa2a37f958ece0fb75c741ecc44fbd2b03516ba3ce87a890fdc5e5de15687
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.707; amd64

### `eclipse-temurin:8u332-b09-jre-nanoserver-ltsc2022` - windows version 10.0.20348.707; amd64

```console
$ docker pull eclipse-temurin@sha256:2a41860544a6178c59902285708f741ce3c84e1dcd9ec2f9e7a3982e4ac42f6a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.0 MB (156989905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56e2d340042dd8b0cde795bbf2e1564a239a8a08b0d5c345dfaba32e1059dda5`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 05 May 2022 02:37:33 GMT
RUN Apply image 10.0.20348.707
# Wed, 11 May 2022 15:21:54 GMT
SHELL [cmd /s /c]
# Wed, 11 May 2022 15:21:55 GMT
ENV JAVA_VERSION=jdk8u332-b09
# Wed, 11 May 2022 15:21:56 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 11 May 2022 15:21:56 GMT
USER ContainerAdministrator
# Wed, 11 May 2022 15:22:12 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 11 May 2022 15:22:13 GMT
USER ContainerUser
# Wed, 11 May 2022 15:23:00 GMT
COPY dir:3ac3da968b0a55dd3b56d678ae78ff2fe7435f143b42a50fa75d097fd864892f in C:\openjdk-8 
# Wed, 11 May 2022 15:23:15 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:2c74f0842c5a8e9b80b9e2cf64e1ab10a6fa67951f28cff5fee060b88128564c`  
		Size: 117.7 MB (117687017 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c783ef8875d74b7e18cf09914325e131a525d4678bc9b243734768fdbcde89a2`  
		Last Modified: Wed, 18 May 2022 13:44:02 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ac36429f933755f4feb3856e62dcb854cd0c3ded07044ef3022b326c9be841`  
		Last Modified: Wed, 18 May 2022 13:44:02 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf983a75185f46dcbd353c4168808c2c98c7bcc1379841008d4f84d61b0e2df`  
		Last Modified: Wed, 18 May 2022 13:44:02 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e08e0e9837cbbdd01d54b4e3bbd7f199b280f70ac9ce2fecc568f676052612`  
		Last Modified: Wed, 18 May 2022 13:44:00 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f802bf7ddce7178c0877e68417448396eea5e1058010f5a9c34b8410373a3d`  
		Last Modified: Wed, 18 May 2022 13:44:00 GMT  
		Size: 99.6 KB (99580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a8ac175dcdbc2fb1317b51dfac0b2b68e6a36afe2e8d00e44514e951e7d6c5`  
		Last Modified: Wed, 18 May 2022 13:44:00 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92f6fb72b2619412dec7d2402a6d9e03cf37121eb98e4094efad9dbe39d8668`  
		Last Modified: Wed, 18 May 2022 13:45:07 GMT  
		Size: 39.1 MB (39128674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15a6427517de7df0383e8640e51c19c9e4622f768939e68c4ebbe4865f7dafb`  
		Last Modified: Wed, 18 May 2022 13:44:25 GMT  
		Size: 68.9 KB (68889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
