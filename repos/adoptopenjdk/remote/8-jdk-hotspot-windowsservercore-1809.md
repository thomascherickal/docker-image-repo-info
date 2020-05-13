## `adoptopenjdk:8-jdk-hotspot-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:abbc3f76c8c34613abc352047096845b8f383032abd87ac61837100aaa831c08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `adoptopenjdk:8-jdk-hotspot-windowsservercore-1809` - windows version 10.0.17763.1217; amd64

```console
$ docker pull adoptopenjdk@sha256:3dfc80de1132d3d56a7950fd469d1174636802868edd1fbd173423018d543975
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1909681058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a7966b993c91a5ab316fddc56a036826f9bdfa894bfc39d600a116ff5e8e26a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 12:41:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 May 2020 16:35:51 GMT
ENV JAVA_VERSION=jdk8u252-b09.1
# Wed, 13 May 2020 16:37:31 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09.1/OpenJDK8U-jdk_x64_windows_hotspot_8u252b09.msi ...');         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09.1/OpenJDK8U-jdk_x64_windows_hotspot_8u252b09.msi -O 'openjdk.msi';         Write-Host ('Verifying sha256 (5a1076e1fc0228b658bd567e7644283ee5169c92ff91460c22caa0c11fde9e4a) ...');         if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '5a1076e1fc0228b658bd567e7644283ee5169c92ff91460c22caa0c11fde9e4a') {                 Write-Host 'FAILED!';                 exit 1;         };                 New-Item -ItemType Directory -Path C:\temp | Out-Null;                 Write-Host 'Installing using MSI ...';         Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',         '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;         Write-Host 'Removing openjdk.msi ...';         Remove-Item openjdk.msi -Force;         Remove-Item -Path C:\temp -Recurse | Out-Null;
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:77613e754ba9d62c0acd4ef271c4ee7d3af091b8c8b310afa404560a9d281f82`  
		Last Modified: Wed, 13 May 2020 13:00:20 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c892583536a813d99404132303d3f4caf4bcb965777d9e40d83aaaf5bb7e2710`  
		Last Modified: Wed, 13 May 2020 17:50:59 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30bae00677c9e954952f997fb2d76323da004afe5106f1f1189e7e66d45b4cb`  
		Last Modified: Wed, 13 May 2020 17:51:29 GMT  
		Size: 191.3 MB (191345881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
