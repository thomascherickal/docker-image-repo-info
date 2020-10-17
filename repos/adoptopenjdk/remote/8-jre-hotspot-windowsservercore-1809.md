## `adoptopenjdk:8-jre-hotspot-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:e82ab01a17da735e032e29ff8f7cf7e44a87771506d09cea45f5a5a668dc5152
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `adoptopenjdk:8-jre-hotspot-windowsservercore-1809` - windows version 10.0.17763.1518; amd64

```console
$ docker pull adoptopenjdk@sha256:6dac991da9a8af07c1adf126d0c549f50045cad9a19b73cecdfb604c622d626a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2456934230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a09690884cfec03bf8b6eb7653d128770c3b945711e3432469ec72b6e349fdd6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 17 Oct 2020 00:14:27 GMT
ENV JAVA_VERSION=jdk8u265-b01
# Sat, 17 Oct 2020 00:51:15 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jre_x64_windows_hotspot_8u265b01.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jre_x64_windows_hotspot_8u265b01.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (5a41ec5d781429b7364412fcb7a05bfd4dd633d9b5e67ab2cdf878ee5ed4c722) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '5a41ec5d781429b7364412fcb7a05bfd4dd633d9b5e67ab2cdf878ee5ed4c722') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
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
	-	`sha256:deb5709d63eb8822ab0607f9e7bf13adeb340973ff7631cead2c9b3cb2524423`  
		Last Modified: Sat, 17 Oct 2020 01:51:29 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14082c96625cc12d8d52dae4a25c8a15b7563b8e0972f405c5017ae3e967ff11`  
		Last Modified: Sat, 17 Oct 2020 01:59:24 GMT  
		Size: 82.8 MB (82841821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
