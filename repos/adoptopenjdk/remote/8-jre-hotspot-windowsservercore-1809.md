## `adoptopenjdk:8-jre-hotspot-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:f818b1fc431f0255ecf1165c00baa291aa8837452da9ac435ceadd138d94f268
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `adoptopenjdk:8-jre-hotspot-windowsservercore-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull adoptopenjdk@sha256:c182703c4ceb1de9184f11315d58657902435f9d8b8c63172766f85e9cb0ea32
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2433924829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a51fdda0aea9e6b4d564266fe7879504b6560d20b6c3e981c4848a4d5c02f72`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 18:00:09 GMT
ENV JAVA_VERSION=jdk8u252-b09.1
# Wed, 09 Sep 2020 18:01:21 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09.1/OpenJDK8U-jre_x64_windows_hotspot_8u252b09.msi ...');         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         wget https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09.1/OpenJDK8U-jre_x64_windows_hotspot_8u252b09.msi -O 'openjdk.msi';         Write-Host ('Verifying sha256 (7651a26e53260e48ca2431a8cdb6b910e8f8c92564cb8378b566d77346a63527) ...');         if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '7651a26e53260e48ca2431a8cdb6b910e8f8c92564cb8378b566d77346a63527') {                 Write-Host 'FAILED!';                 exit 1;         };                 New-Item -ItemType Directory -Path C:\temp | Out-Null;                 Write-Host 'Installing using MSI ...';         Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',         '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;         Write-Host 'Removing openjdk.msi ...';         Remove-Item openjdk.msi -Force;         Remove-Item -Path C:\temp -Recurse | Out-Null;
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff6523146333d114d974e2cfedc2baf6d52ab8a40d312446622f31e935b138b`  
		Last Modified: Wed, 09 Sep 2020 19:13:24 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61507f07690d132fe9aafc261bfa5fb44b90077b1961b6a492ad4cda8e2ae83`  
		Last Modified: Wed, 09 Sep 2020 19:14:57 GMT  
		Size: 82.7 MB (82650333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
