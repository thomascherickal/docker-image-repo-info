## `adoptopenjdk:14-jre-hotspot-windowsservercore`

```console
$ docker pull adoptopenjdk@sha256:9eb05b4d1d474ea272deb55146dc3ff23e55929fae864686bb63f10d133b4d8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3686; amd64
	-	windows version 10.0.17763.1217; amd64

### `adoptopenjdk:14-jre-hotspot-windowsservercore` - windows version 10.0.14393.3686; amd64

```console
$ docker pull adoptopenjdk@sha256:7a7322eef00cf50e62fc756b68af53d4b66cf31f54e609ac87d12f98f9d15740
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5830671362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e21b86192bd40444b00ac01b0965de2133b296c240f62cb4abbded0e4f173d59`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 04 May 2020 15:24:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 May 2020 12:34:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 May 2020 17:00:39 GMT
ENV JAVA_VERSION=jdk-14.0.1+7.1
# Wed, 13 May 2020 17:09:02 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.1%2B7.1/OpenJDK14U-jre_x64_windows_hotspot_14.0.1_7.msi ...');         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         wget https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.1%2B7.1/OpenJDK14U-jre_x64_windows_hotspot_14.0.1_7.msi -O 'openjdk.msi';         Write-Host ('Verifying sha256 (b89f20b57a87c41f0838d962768a40dac826baa4bc2fe76f3934d0919a096abd) ...');         if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'b89f20b57a87c41f0838d962768a40dac826baa4bc2fe76f3934d0919a096abd') {                 Write-Host 'FAILED!';                 exit 1;         };                 New-Item -ItemType Directory -Path C:\temp | Out-Null;                 Write-Host 'Installing using MSI ...';         Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',         '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;         Write-Host 'Removing openjdk.msi ...';         Remove-Item openjdk.msi -Force;         Remove-Item -Path C:\temp -Recurse | Out-Null;
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b940e70a4619b357d89f3dcabf4ac263d1efc65e1ef3af64cb0e8fbeaccc64dd`  
		Size: 1.7 GB (1661903967 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e3e9730c43354781e87aa51e853bff3b1e8c1ca7004f527139638a8f9d499c49`  
		Last Modified: Wed, 13 May 2020 12:59:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b15f5cd3b37c0e2efddc70f4e39ce025783e5f52cc92e2194b4243f666f18eb`  
		Last Modified: Wed, 13 May 2020 18:13:06 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26cd3ba71e0a251ca9c0d79752566dc542acba3c76602bae422bd00b689ff125`  
		Last Modified: Wed, 13 May 2020 18:17:42 GMT  
		Size: 98.8 MB (98779216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:14-jre-hotspot-windowsservercore` - windows version 10.0.17763.1217; amd64

```console
$ docker pull adoptopenjdk@sha256:d070ca6e5a27a181241cba4a221e7c0f49a8b88626927f2d8a5c7a0e1ce779a7
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1812127629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83159a9ce6b6eb7186908930c9d1c3a5df8b43dcaba6e8b3c5a9c58f4d07c110`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 12:41:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 May 2020 17:04:22 GMT
ENV JAVA_VERSION=jdk-14.0.1+7.1
# Wed, 13 May 2020 17:10:25 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.1%2B7.1/OpenJDK14U-jre_x64_windows_hotspot_14.0.1_7.msi ...');         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         wget https://github.com/AdoptOpenJDK/openjdk14-binaries/releases/download/jdk-14.0.1%2B7.1/OpenJDK14U-jre_x64_windows_hotspot_14.0.1_7.msi -O 'openjdk.msi';         Write-Host ('Verifying sha256 (b89f20b57a87c41f0838d962768a40dac826baa4bc2fe76f3934d0919a096abd) ...');         if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'b89f20b57a87c41f0838d962768a40dac826baa4bc2fe76f3934d0919a096abd') {                 Write-Host 'FAILED!';                 exit 1;         };                 New-Item -ItemType Directory -Path C:\temp | Out-Null;                 Write-Host 'Installing using MSI ...';         Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',         '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;         Write-Host 'Removing openjdk.msi ...';         Remove-Item openjdk.msi -Force;         Remove-Item -Path C:\temp -Recurse | Out-Null;
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:77613e754ba9d62c0acd4ef271c4ee7d3af091b8c8b310afa404560a9d281f82`  
		Last Modified: Wed, 13 May 2020 13:00:20 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09430b3fa3b258d3b5d8b30b569d7294b5e692d020988cbc6cff05cbb93d261d`  
		Last Modified: Wed, 13 May 2020 18:14:17 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd629949478bedb635e634e2c5c2aea8711a9bd7d5004628e59bf6c2b20d1063`  
		Last Modified: Wed, 13 May 2020 18:18:04 GMT  
		Size: 93.8 MB (93792460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
