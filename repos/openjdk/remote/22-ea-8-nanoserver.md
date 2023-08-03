## `openjdk:22-ea-8-nanoserver`

```console
$ docker pull openjdk@sha256:862abb8f69ce57dcf2e879c2065d3435610a314d6859561fd427ac9b252c68fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4645; amd64

### `openjdk:22-ea-8-nanoserver` - windows version 10.0.17763.4645; amd64

```console
$ docker pull openjdk@sha256:8fa6d2cb9c18b8c9545a0ab4e84722790ab4c1f7cce1107bd834d25150a9004d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.1 MB (307142377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb3f53192a532e34c65cea6cbfd7827c3763f31f4402f0fe204c64c6a20bd5cc`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 07 Jul 2023 07:42:59 GMT
RUN Apply image 10.0.17763.4645
# Thu, 13 Jul 2023 21:36:32 GMT
SHELL [cmd /s /c]
# Fri, 14 Jul 2023 00:14:58 GMT
ENV JAVA_HOME=C:\openjdk-22
# Fri, 14 Jul 2023 00:14:58 GMT
USER ContainerAdministrator
# Fri, 14 Jul 2023 00:15:08 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Fri, 14 Jul 2023 00:15:09 GMT
USER ContainerUser
# Thu, 03 Aug 2023 01:00:24 GMT
ENV JAVA_VERSION=22-ea+8
# Thu, 03 Aug 2023 01:00:39 GMT
COPY dir:844ed35e292afeef7618734fa3174c636b1fcb1ca47d76affcc8af1c07d3061e in C:\openjdk-22 
# Thu, 03 Aug 2023 01:00:50 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Thu, 03 Aug 2023 01:00:51 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5c5b06ba65934bcf850a1a54ecf4b3da34d3e6d6c8e90dbc897719c3ea377c8a`  
		Last Modified: Tue, 11 Jul 2023 17:31:37 GMT  
		Size: 104.4 MB (104408241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13c473988daf5951866dd9b290bd6417227c1d7df6e811cfe11438d033a1eba`  
		Last Modified: Thu, 13 Jul 2023 22:19:06 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544d6fd540738704e91e0cdf5ce429fe06193ca6f57b912ecd37720a5398c73e`  
		Last Modified: Fri, 14 Jul 2023 00:23:01 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184aebbaa7a5b561357f50ab1e278ddea12853b5513f6ccee076e8977ee17cb5`  
		Last Modified: Fri, 14 Jul 2023 00:23:00 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f517a720df0787d39ebc3c54f30149bad465e8af46947e6dd7c609c5c63d3ef3`  
		Last Modified: Fri, 14 Jul 2023 00:23:00 GMT  
		Size: 71.4 KB (71362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ee6f2b90fa1d7c818530d35c4808f44d5fa2414919c02d26f5b7db881751ed`  
		Last Modified: Fri, 14 Jul 2023 00:22:58 GMT  
		Size: 1.1 KB (1115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e286bd418e85b39840243f49e034b73137a3e10cfb9388d2ece9747d4ec59651`  
		Last Modified: Thu, 03 Aug 2023 01:41:10 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dae5b57c2a760c7583075a715c1953553825d9e8bb2616c36fc19eafe86c53c`  
		Last Modified: Thu, 03 Aug 2023 01:41:32 GMT  
		Size: 198.8 MB (198839044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c834558bb8c8a8cb8f36df3075c2611c26549bfeaa45085a223921f73390d7a2`  
		Last Modified: Thu, 03 Aug 2023 01:41:12 GMT  
		Size: 3.8 MB (3816946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a6a2d44d2f738618a50c9e2b7de8acfb2ffc4934f951716cb816112de25e42`  
		Last Modified: Thu, 03 Aug 2023 01:41:10 GMT  
		Size: 1.1 KB (1062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
