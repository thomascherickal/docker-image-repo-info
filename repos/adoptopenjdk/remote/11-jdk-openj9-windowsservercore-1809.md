## `adoptopenjdk:11-jdk-openj9-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:ba27f6e9b49f410692b924fbac21e7266d41b86b17f17d093474dde6507326d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `adoptopenjdk:11-jdk-openj9-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull adoptopenjdk@sha256:5ff0698684ae9318d2a1da11880e043a402e83e750be71bf8b1278ad37fec97e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2841284225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed975aac88624d86cd21cdff26c4603755841197f363f486480173ee19b3b690`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 19:58:53 GMT
ENV JAVA_VERSION=jdk-11.0.10+9_openj9-0.24.0
# Wed, 10 Mar 2021 20:00:36 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jdk_x64_windows_openj9_11.0.10_9_openj9-0.24.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jdk_x64_windows_openj9_11.0.10_9_openj9-0.24.0.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (f0abd0ad0fcecb0afee310d19655db680b2758f015d26bbb28ca50eaf263b09c) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'f0abd0ad0fcecb0afee310d19655db680b2758f015d26bbb28ca50eaf263b09c') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 10 Mar 2021 20:00:38 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Wed, 10 Mar 2021 20:00:39 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9187e1445ac8523738bcb8db3256dc65ae6c632a2bf351d3a4540af5d3e8e584`  
		Last Modified: Wed, 10 Mar 2021 21:04:49 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ed7759031ff681477eafb3211595ff64f5d9f47983ce001bfa289e040832ff`  
		Last Modified: Wed, 10 Mar 2021 21:05:26 GMT  
		Size: 379.7 MB (379744028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14e7cc0608a1520f8dde930fc368b86b18a7be498194c2765173cc79cb4f39a`  
		Last Modified: Wed, 10 Mar 2021 21:04:49 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9ec49a8f94797e25648da2a44c4c7a51d49920d7e36999e51c0655d8cef2d6`  
		Last Modified: Wed, 10 Mar 2021 21:04:49 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
