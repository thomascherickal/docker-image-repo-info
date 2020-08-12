## `openjdk:16-ea-9-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:e901afca812db08f807a4f53df7c6ed7e699c26c27bc3471d88bfb51b5e63007
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `openjdk:16-ea-9-jdk-nanoserver-1809` - windows version 10.0.17763.1397; amd64

```console
$ docker pull openjdk@sha256:4cc1ce4d397d9359f7749143e10c6bfd59dfcb25566412fa98fe47a754c370ba
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.8 MB (296759055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e9be1b3f325672980598de81340c306e6f1fc072f4610e16467fa3a45da3288`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 06 Aug 2020 01:28:42 GMT
RUN Apply image 1809-amd64
# Wed, 12 Aug 2020 15:28:05 GMT
SHELL [cmd /s /c]
# Wed, 12 Aug 2020 15:28:06 GMT
ENV JAVA_HOME=C:\openjdk-16
# Wed, 12 Aug 2020 15:28:06 GMT
USER ContainerAdministrator
# Wed, 12 Aug 2020 15:28:21 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Wed, 12 Aug 2020 15:28:22 GMT
USER ContainerUser
# Wed, 12 Aug 2020 15:28:23 GMT
ENV JAVA_VERSION=16-ea+9
# Wed, 12 Aug 2020 15:29:02 GMT
COPY dir:e2d94f447255630b2f23327408c6183bf8ac1833da5fb2b9945a4c90e6940da7 in C:\openjdk-16 
# Wed, 12 Aug 2020 15:29:24 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Wed, 12 Aug 2020 15:29:25 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:ce1c649a3e5b5b5449776d4afce631c673cade12336ccb5a38a0aac7c9d8b2bc`  
		Size: 101.0 MB (100984944 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1c7c341c7a3d0c7b6e849b6faec560815682d07ce87df2e4d1e83f928aab306b`  
		Last Modified: Wed, 12 Aug 2020 16:10:21 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4ff90b84cb0e951da0f399342768862ac8c294fbe71e80d787a60d9cc2c7b5`  
		Last Modified: Wed, 12 Aug 2020 16:10:20 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f566429948e6233b746b6d219e57703486a6f2f00910b8e1842ff9920d1834e1`  
		Last Modified: Wed, 12 Aug 2020 16:10:20 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a4bcc2b175dfe1adf68a872a4fa40033320f09b67b59f3dbf35cae4783189d4`  
		Last Modified: Wed, 12 Aug 2020 16:10:20 GMT  
		Size: 65.9 KB (65918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ca4105c8d6a5159a2ffd6904f118076cb11506891820a04656978435fd29bad`  
		Last Modified: Wed, 12 Aug 2020 16:10:17 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9358d8c8fe5ca782d3a9911b948613aff3c2e74f7b16725b35bf3809f8984622`  
		Last Modified: Wed, 12 Aug 2020 16:10:17 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a24c06f2b06c38f6627141b02bb472cb4091d84153390cb594ab143139146f`  
		Last Modified: Wed, 12 Aug 2020 16:10:37 GMT  
		Size: 192.2 MB (192171434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c813d66bb2e7dee165c72c6e8fc388bf33cf0ad6a19b82922c5896224290978`  
		Last Modified: Wed, 12 Aug 2020 16:10:18 GMT  
		Size: 3.5 MB (3531507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad0f96ba8e106e426bfea8d75a591d25fc3d4258502e0d42407d2a9d25008bc`  
		Last Modified: Wed, 12 Aug 2020 16:10:17 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
