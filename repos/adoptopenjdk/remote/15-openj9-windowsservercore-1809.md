## `adoptopenjdk:15-openj9-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:830ea13f9b08f13f04a6459031bfff17ce7e0f856e727236125e87842e44f3ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `adoptopenjdk:15-openj9-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull adoptopenjdk@sha256:d809cc308fe116ec76ca37d49f09f5061eb52865602f00eaffa23c368e619721
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2772878324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d619fe6744a5f1a28a4b4a7c39278656c929139069fc55bcc330de8df9549099`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 13:30:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 21:32:15 GMT
ENV JAVA_VERSION=jdk-15.0.1+9_openj9-0.23.0
# Wed, 09 Dec 2020 21:34:40 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9_openj9-0.23.0/OpenJDK15U-jdk_x64_windows_openj9_15.0.1_9_openj9-0.23.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9_openj9-0.23.0/OpenJDK15U-jdk_x64_windows_openj9_15.0.1_9_openj9-0.23.0.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (6745ab134f86bdb27154800fd0164a6d957c31a78a2cd812234d3c25639b0bf9) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '6745ab134f86bdb27154800fd0164a6d957c31a78a2cd812234d3c25639b0bf9') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 09 Dec 2020 21:34:41 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Wed, 09 Dec 2020 21:34:42 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a4372d14958dc8a7eaaace9e4774e7f1db524da5eb4474b5e46738848a3a61a5`  
		Last Modified: Wed, 09 Dec 2020 13:54:38 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c1639431fca3978429c18a7f57b4a2f34f60e75472ae76f2c5b97f194496a7`  
		Last Modified: Wed, 09 Dec 2020 22:28:18 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34371951c5bd130a0227aa0c6371873df8de370d9f313991501289b07f83c692`  
		Last Modified: Wed, 09 Dec 2020 22:35:38 GMT  
		Size: 382.0 MB (381999446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a673171b091dae2aa3575cccf54eaaafd59c9d9b957858e38870c826d450cd4f`  
		Last Modified: Wed, 09 Dec 2020 22:28:18 GMT  
		Size: 1.1 KB (1083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e083a450e3cf694c72f44d6c144d80e0f4fbe4e2c83ebda69d87bce5e692563`  
		Last Modified: Wed, 09 Dec 2020 22:28:18 GMT  
		Size: 1.1 KB (1075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
