## `adoptopenjdk:15-jdk-openj9-windowsservercore`

```console
$ docker pull adoptopenjdk@sha256:438c5c871d2f216cc0d4f69daee871f79c48a4c194c2f04fe757157d9f7235a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64
	-	windows version 10.0.14393.3986; amd64

### `adoptopenjdk:15-jdk-openj9-windowsservercore` - windows version 10.0.17763.1518; amd64

```console
$ docker pull adoptopenjdk@sha256:02cc5dd05846a187738bfd93f4a2eede6fb5b89f1bcc89ca9ab1d8e9a263716b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2756017250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86a77a72d6206b17429b2a5e5fc491ba1743f2a16038f49aa88661ecb90be53e`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 17 Oct 2020 01:34:37 GMT
ENV JAVA_VERSION=jdk-15+36_openj9-0.22.0
# Sat, 17 Oct 2020 01:37:28 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36_openj9-0.22.0/OpenJDK15U-jdk_x64_windows_openj9_15_36_openj9-0.22.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36_openj9-0.22.0/OpenJDK15U-jdk_x64_windows_openj9_15_36_openj9-0.22.0.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (88dd04dc008ff18e09ad158046a650797ff8e5ce0f1880515e359c49f0fddd4e) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '88dd04dc008ff18e09ad158046a650797ff8e5ce0f1880515e359c49f0fddd4e') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Sat, 17 Oct 2020 01:37:29 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Sat, 17 Oct 2020 01:37:30 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5e61fff845eda39f31bdf5d797254fdf656ee79d8c294c1713007864bc4c2535`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b72aeaa8c42cf486f1e47e7b58d97f365ca33f5f183447aa42a4f296e2bd85b`  
		Last Modified: Sat, 17 Oct 2020 02:22:42 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59149a8e1a4d595880d79b242a53396b588c5a52667dceac1d6294e6fe4de019`  
		Last Modified: Sat, 17 Oct 2020 02:23:10 GMT  
		Size: 381.9 MB (381922588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83c6028ca1988dec1ef628f1afc872acc805099e47d6b79488813cf4470e838`  
		Last Modified: Sat, 17 Oct 2020 02:22:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b18514c1fb7253e06e7133b6a8f2a9453d90e82f938b1754cb861b2d48ac55`  
		Last Modified: Sat, 17 Oct 2020 02:22:42 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:15-jdk-openj9-windowsservercore` - windows version 10.0.14393.3986; amd64

```console
$ docker pull adoptopenjdk@sha256:f5957d7c096b4cfe8fbb50dc5867a5cd51a7a03d1e1b7485740ef3356bb6ab77
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6123906946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5f7eefa084b3e3ec198004f25f29ed99e746049d97e6ca98faea92398277d09`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 17 Oct 2020 01:37:37 GMT
ENV JAVA_VERSION=jdk-15+36_openj9-0.22.0
# Sat, 17 Oct 2020 01:41:00 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36_openj9-0.22.0/OpenJDK15U-jdk_x64_windows_openj9_15_36_openj9-0.22.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36_openj9-0.22.0/OpenJDK15U-jdk_x64_windows_openj9_15_36_openj9-0.22.0.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (88dd04dc008ff18e09ad158046a650797ff8e5ce0f1880515e359c49f0fddd4e) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '88dd04dc008ff18e09ad158046a650797ff8e5ce0f1880515e359c49f0fddd4e') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Sat, 17 Oct 2020 01:41:01 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Sat, 17 Oct 2020 01:41:02 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e300a13db0fbbf48a676ace9db3b0de292c825dfa01e6d82979d96ebc23d3675`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:086d2ce2178c7eb1c489e3433b970bcb6bfbdb0a09a5c7a1a108e787f63973a8`  
		Last Modified: Sat, 17 Oct 2020 02:23:40 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c377a2f5b23560dee15fcef3762e2741e7e2c5f892ae936e4a1f64cbe0dc30`  
		Last Modified: Sat, 17 Oct 2020 02:24:23 GMT  
		Size: 382.6 MB (382550751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc49d6979355ee36af04e2d228dba89b6516f7ba0a719b56fbafe46a264d41ce`  
		Last Modified: Sat, 17 Oct 2020 02:23:40 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cf4dfaf2158f06d28b4b7b43441e3f45d1562e3f2db31a8a70941782bc0a402`  
		Last Modified: Sat, 17 Oct 2020 02:23:41 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
