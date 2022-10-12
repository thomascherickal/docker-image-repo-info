## `golang:nanoserver-ltsc2022`

```console
$ docker pull golang@sha256:06aa3c2751a788da2c8e38d82ddde1f5cc4182ee763316b1fef118ba3519cf68
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1129; amd64

### `golang:nanoserver-ltsc2022` - windows version 10.0.20348.1129; amd64

```console
$ docker pull golang@sha256:79867343ee8d01588a1d7c6b439ec80b10030b2e5c0cf66a52edd23cd2c90600
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.6 MB (275622803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:089bd9f5bdd52378dd83971aab0cc0395b8cc7a7bea22729b712be66518c1a80`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Fri, 07 Oct 2022 21:37:41 GMT
RUN Apply image 10.0.20348.1129
# Wed, 12 Oct 2022 12:51:25 GMT
SHELL [cmd /S /C]
# Wed, 12 Oct 2022 12:51:26 GMT
ENV GOPATH=C:\go
# Wed, 12 Oct 2022 12:51:26 GMT
USER ContainerAdministrator
# Wed, 12 Oct 2022 12:52:17 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Wed, 12 Oct 2022 12:52:17 GMT
USER ContainerUser
# Wed, 12 Oct 2022 12:52:18 GMT
ENV GOLANG_VERSION=1.19.2
# Wed, 12 Oct 2022 12:54:51 GMT
COPY dir:1fc645e1b9a8ffb5757805e06eefa6c9c9b0f649b5403eeab554ede8594c418b in C:\Program Files\Go 
# Wed, 12 Oct 2022 12:55:42 GMT
RUN go version
# Wed, 12 Oct 2022 12:55:42 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:38fa349577729651ac1fc3ec785f908719a8100da5f5ba9bd3f549411061f583`  
		Size: 118.2 MB (118202895 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c9abf6e1518124a035a9bbaf0dad0924d5286be7dc0ee052f1225355c2e68da7`  
		Last Modified: Wed, 12 Oct 2022 13:17:17 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1a05eb086128aa5209bbd6a53d080b706f5ba02d90319bac1ae748bd277b59`  
		Last Modified: Wed, 12 Oct 2022 13:17:17 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e6cf59dc3a7ca9816cacef203e2e6a8a4cde3060b92affa21d3bb48afe3ac78`  
		Last Modified: Wed, 12 Oct 2022 13:17:17 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48576001e81f34a54b49993c9d72be646fbb21c51288f1bff0dc553c777f83a2`  
		Last Modified: Wed, 12 Oct 2022 13:17:17 GMT  
		Size: 85.9 KB (85857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fbc6112ad01bb79cdee313cd41d392c340336479be92f8fd30e677bc61543be`  
		Last Modified: Wed, 12 Oct 2022 13:17:14 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2902450e123a6951b05518729277298f62d6e0255cc6200797a5a702b893af6`  
		Last Modified: Wed, 12 Oct 2022 13:17:15 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89b6fd5511cae06061fc33e91f497970ac5124b5e8ddffbd798f24bf52fd122`  
		Last Modified: Wed, 12 Oct 2022 13:17:53 GMT  
		Size: 157.3 MB (157277598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7871e36033162fff5adbd436d0cec91f27f457308c9580d7fdebe0ed8aa3fdd0`  
		Last Modified: Wed, 12 Oct 2022 13:17:14 GMT  
		Size: 49.3 KB (49285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b75acbff5494f9682162805ce08b562e0ec220018217c38f3f0d4468fcee95f`  
		Last Modified: Wed, 12 Oct 2022 13:17:14 GMT  
		Size: 1.4 KB (1350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
