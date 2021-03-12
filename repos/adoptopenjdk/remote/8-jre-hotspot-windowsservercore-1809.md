## `adoptopenjdk:8-jre-hotspot-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:93a9f0b83de02ac87ee6224e80d8824dc3f0b05335b029943252807429dc5634
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `adoptopenjdk:8-jre-hotspot-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull adoptopenjdk@sha256:daf5cd34060c63f93f605a0807edab61689f780fbbb6b9aba7e59146cb6c89ae
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2545263154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:606d44e7445a10750bc9b642db9aba73789d4283e01ce2bbae8de7049705e2e6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 18:58:24 GMT
ENV JAVA_VERSION=jdk8u282-b08
# Wed, 10 Mar 2021 19:10:23 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u282-b08/OpenJDK8U-jre_x64_windows_hotspot_8u282b08.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u282-b08/OpenJDK8U-jre_x64_windows_hotspot_8u282b08.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (edb227414937de5024c70eb1f50406fdcad96c4dce1c9bf866b9396dde08b462) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'edb227414937de5024c70eb1f50406fdcad96c4dce1c9bf866b9396dde08b462') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
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
	-	`sha256:842ee128f60e6e47d30b23fa3de6f12a1b5df1a97cf9a77f57d99770469d8148`  
		Last Modified: Wed, 10 Mar 2021 20:28:43 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c33e8a702334ed65893057072ddc1d0c0619981d0266bc60843122bae30847`  
		Last Modified: Wed, 10 Mar 2021 20:33:43 GMT  
		Size: 83.7 MB (83725854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
