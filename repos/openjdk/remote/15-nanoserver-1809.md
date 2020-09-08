## `openjdk:15-nanoserver-1809`

```console
$ docker pull openjdk@sha256:d6dfc6b7aaa202a12c0ba7f4e96c3c603f30201d3cbe5f8f736b1cd4ccf49381
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `openjdk:15-nanoserver-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull openjdk@sha256:028439c95a5123b249437ee07975ad5473e89350d4e6ef0f9dbe44b9b8a0ed9d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.2 MB (296188682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:889725aed6194737fe7d632e7d2faea2e2f4f1e394c39fcad3cfef12280433db`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 02 Sep 2020 12:08:18 GMT
RUN Apply image 1809-amd64
# Tue, 08 Sep 2020 20:13:38 GMT
SHELL [cmd /s /c]
# Tue, 08 Sep 2020 20:21:59 GMT
ENV JAVA_HOME=C:\openjdk-15
# Tue, 08 Sep 2020 20:22:00 GMT
USER ContainerAdministrator
# Tue, 08 Sep 2020 20:22:10 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Tue, 08 Sep 2020 20:22:11 GMT
USER ContainerUser
# Tue, 08 Sep 2020 20:22:11 GMT
ENV JAVA_VERSION=15
# Tue, 08 Sep 2020 20:22:49 GMT
COPY dir:c7e08674451932ee3e39dd647bf57a58f604f71d6631e01f3c30405731e02d63 in C:\openjdk-15 
# Tue, 08 Sep 2020 20:23:10 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Tue, 08 Sep 2020 20:23:11 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:ecf9bb62dc6eedea9fd367628f8715dea75b7d2053afa4b5121e7809aa692139`  
		Size: 101.2 MB (101239122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f72ec155bceaba8b4a5cdbd7aa79586c7296a801af5364a691c46191c910e2da`  
		Last Modified: Tue, 08 Sep 2020 22:29:01 GMT  
		Size: 864.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2217be67cc2e5e1e1a3cef8c65a2d0320eac1bb80a6ddce61e1c8e08f9af5858`  
		Last Modified: Tue, 08 Sep 2020 22:32:54 GMT  
		Size: 865.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e55a8c4b633f6ecc66ceedb0392b2a43b01eddebe7329120c3a137cc1aa4d49`  
		Last Modified: Tue, 08 Sep 2020 22:32:54 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eedb0918a66506aebf1473a555fbb168ad7996c6cd6020926984af40fab93c49`  
		Last Modified: Tue, 08 Sep 2020 22:32:54 GMT  
		Size: 66.5 KB (66514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:487d87f337f554619e23049b0973899904700ec75d46907c29125ba22978735f`  
		Last Modified: Tue, 08 Sep 2020 22:32:51 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab682931656368a8e60c422c4ad34b999ecf570f526bc0329d655dba93d1995`  
		Last Modified: Tue, 08 Sep 2020 22:32:51 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2f0483aa4c54effc236eae8064c47a56e94b0bcdd54655d1774c3ab98e767c`  
		Last Modified: Tue, 08 Sep 2020 22:33:10 GMT  
		Size: 191.4 MB (191359189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac3b73fbf5f80c3cb4d983f19a6324c3c39f9fbaf08ba2fd87a1fe27f9af040`  
		Last Modified: Tue, 08 Sep 2020 22:32:52 GMT  
		Size: 3.5 MB (3518575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e72160303a803925e5e92190f9264f86d40cf4382d9ab237fccef699c960ba`  
		Last Modified: Tue, 08 Sep 2020 22:32:51 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
