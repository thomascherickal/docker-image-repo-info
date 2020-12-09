## `adoptopenjdk:openj9-windowsservercore`

```console
$ docker pull adoptopenjdk@sha256:95878ce5d5610bbdae878c6525cebaae25b7ee9fc85162bacad9517d2f631123
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `adoptopenjdk:openj9-windowsservercore` - windows version 10.0.17763.1637; amd64

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

### `adoptopenjdk:openj9-windowsservercore` - windows version 10.0.14393.4104; amd64

```console
$ docker pull adoptopenjdk@sha256:fc9b1cc335aee6e838ab2677ed6b9f642247a5fb3b1147460432fa5347ad2951
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6151604489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:470c97eac030eeab63fb993b23f49683c42fa83c8e5091d5200a17dbd19718c9`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 13:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 21:34:58 GMT
ENV JAVA_VERSION=jdk-15.0.1+9_openj9-0.23.0
# Wed, 09 Dec 2020 21:38:01 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9_openj9-0.23.0/OpenJDK15U-jdk_x64_windows_openj9_15.0.1_9_openj9-0.23.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9_openj9-0.23.0/OpenJDK15U-jdk_x64_windows_openj9_15.0.1_9_openj9-0.23.0.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (6745ab134f86bdb27154800fd0164a6d957c31a78a2cd812234d3c25639b0bf9) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '6745ab134f86bdb27154800fd0164a6d957c31a78a2cd812234d3c25639b0bf9') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 09 Dec 2020 21:38:02 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Wed, 09 Dec 2020 21:38:03 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c6d005eb9e78ad42f77f3dad7e29d954e78f0547f9884fe024a71f4042412970`  
		Last Modified: Wed, 09 Dec 2020 13:55:31 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7936991db76fe16143811b69d35d076062f0c0f45e89d8afad60c9b2299a5380`  
		Last Modified: Wed, 09 Dec 2020 22:35:56 GMT  
		Size: 1.1 KB (1082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02af2d0ba92288db9bedd845ff9a9b3da78b0925c97dcd6a17caeda7254a49fd`  
		Last Modified: Wed, 09 Dec 2020 22:36:25 GMT  
		Size: 382.8 MB (382755944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539e6dc26d3ec6ecb60651083eb636767b45de45235355c4e57fe2503836193d`  
		Last Modified: Wed, 09 Dec 2020 22:35:57 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9758a8c69ab28a812f1f7385e354fb842138a49c2a1b9e4eb5d743c52eadf6e9`  
		Last Modified: Wed, 09 Dec 2020 22:35:56 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
