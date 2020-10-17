## `adoptopenjdk:15-jre-openj9-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:13b88c0be82c2c29d8d63ab5c7f613cf2d36dbea4e20c3a457e2daa32e20655f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `adoptopenjdk:15-jre-openj9-windowsservercore-1809` - windows version 10.0.17763.1518; amd64

```console
$ docker pull adoptopenjdk@sha256:250c9e5a2ddb844d2237ebb4c8db7e82e8b893f3f197e02afb291e9e7f5ed425
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2468317828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c3fea768498a3026204bdc83d3b82bd0ac9d136653d93fe31226ba92ab642d5`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
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
# Sat, 17 Oct 2020 01:42:54 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36_openj9-0.22.0/OpenJDK15U-jre_x64_windows_openj9_15_36_openj9-0.22.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36_openj9-0.22.0/OpenJDK15U-jre_x64_windows_openj9_15_36_openj9-0.22.0.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (78b7f6950c5afafa99164644f8dc85cd05d653964e828b52ea1916a3e27b7e61) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '78b7f6950c5afafa99164644f8dc85cd05d653964e828b52ea1916a3e27b7e61') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Sat, 17 Oct 2020 01:42:55 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
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
	-	`sha256:874769c9be32caddbcefde8f29448dc0374a4aa28de3dfa8cbc89bf3da29580b`  
		Last Modified: Sat, 17 Oct 2020 02:24:56 GMT  
		Size: 94.2 MB (94224264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e0f8df37e78547fe88f6dd16372ce138dcfd1fed7f7259c2da9af97049ab9be`  
		Last Modified: Sat, 17 Oct 2020 02:24:43 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
