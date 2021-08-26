## `eclipse-temurin:8u302-b08-jre-windowsservercore-1809`

```console
$ docker pull eclipse-temurin@sha256:67722131005ca8bfd15d12ef096f498395f1b027bfe42a2724e4ea192966b56a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `eclipse-temurin:8u302-b08-jre-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull eclipse-temurin@sha256:c4e8522ef7992585bbbee661f76a964092745f4bb4674c61223edf2201bfce56
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2756964858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f252712b0412b9611a0ff500df310e801e4b0798dbf1f91aa9911f9671b4338`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Tue, 24 Aug 2021 23:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 25 Aug 2021 16:29:13 GMT
ENV JAVA_VERSION=jdk8u302-b08
# Wed, 25 Aug 2021 16:36:04 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_windows_hotspot_8u302b08.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_windows_hotspot_8u302b08.msi ;     Write-Host ('Verifying sha256 (34e5eea737dfaca57ec5162e6fece5259f403fa419c7bcab572e9cdd2bcf8dd1) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '34e5eea737dfaca57ec5162e6fece5259f403fa419c7bcab572e9cdd2bcf8dd1') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {             Write-Host 'FAILED installing MSI!' ;             exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 25 Aug 2021 16:37:02 GMT
RUN Write-Host 'Verifying install ...';     Write-Host '  java -version'; java -version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:547a42a22856b8c453f88ea7796b08c15b248d73f09976ca0044162fb9d12390`  
		Last Modified: Tue, 24 Aug 2021 23:25:12 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf5ffaf540fdab4c73913780b326ca2cb2c5a0f61040fdb1c0e6aeaf9d2f768`  
		Last Modified: Wed, 25 Aug 2021 23:17:07 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958065d0f6bd35172637431a0a502ef37aebf17ed70bf626f0ddfe945b3b787f`  
		Last Modified: Wed, 25 Aug 2021 23:24:23 GMT  
		Size: 70.6 MB (70619684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b0811547331e5d0fe4868a358ef8141a130ede356f24c87074f49b480cd3808`  
		Last Modified: Wed, 25 Aug 2021 23:23:11 GMT  
		Size: 344.4 KB (344386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
