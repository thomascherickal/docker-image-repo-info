## `julia:1-windowsservercore-ltsc2016`

```console
$ docker pull julia@sha256:fcc13ec2a4deabaf456332de57a4deb15d8de966d654c531dc259215595aa7a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3384; amd64

### `julia:1-windowsservercore-ltsc2016` - windows version 10.0.14393.3384; amd64

```console
$ docker pull julia@sha256:4466de07b40c1ccef59af3ba9657c9bd0860ae48a5c64905996975fd98c36c8f
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5851253362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e052b93d9ffa13c50ad0cc5a1adf4bc81224f0ecb84bf49897c21f470ff7ba2e`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 00:35:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Dec 2019 18:12:36 GMT
ENV JULIA_VERSION=1.3.0
# Wed, 11 Dec 2019 18:12:37 GMT
ENV JULIA_SHA256=35af4b93188b2404a78026b583c7f010ecb17df2eabb9fc32de4737de28f31d5
# Wed, 11 Dec 2019 18:16:16 GMT
RUN $url = ('https://julialang-s3.julialang.org/bin/winnt/x64/{1}/julia-{0}-win64.exe' -f $env:JULIA_VERSION, ($env:JULIA_VERSION.Split('.')[0..1] -Join '.'));         Write-Host ('Downloading {0} ...' -f $url);         [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;         Invoke-WebRequest -Uri $url -OutFile 'julia.exe';                 Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256);         if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) {                 Write-Host 'FAILED!';                 exit 1;         };                 Write-Host 'Installing ...';         Start-Process -Wait -NoNewWindow                 -FilePath '.\julia.exe'                 -ArgumentList @(                         '/S',                         '/D=C:\julia'                 );                 Write-Host 'Updating PATH ...';         $env:PATH = 'C:\julia\bin;' + $env:PATH;         [Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine);                 Write-Host 'Verifying install ("julia --version") ...';         julia --version;                 Write-Host 'Removing ...';         Remove-Item julia.exe -Force;                 Write-Host 'Complete.'
# Wed, 11 Dec 2019 18:16:17 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:530e4240d4261ce165890648d1df6230dc4f9ce5df2e6cf9f0d5876694c3d4f0`  
		Last Modified: Wed, 11 Dec 2019 01:14:39 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bb6a227a3e35a2ac1412d7ce1f6d1fe0eb9ffef54d7fd0d942eda6a4a9e844`  
		Last Modified: Wed, 11 Dec 2019 18:20:30 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895110186ac4672791f3312f5bb04163342b724e9e41e75ef5a12770627e6f6a`  
		Last Modified: Wed, 11 Dec 2019 18:20:30 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87adc6544f789d6c8a086e47e9cd0e80a1fae0c26a74b3bd0c4362a9ba35ce65`  
		Last Modified: Wed, 11 Dec 2019 18:21:07 GMT  
		Size: 128.5 MB (128544729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a92f8fb56b5bcfe5c53c100e5ce668116c15207c92ed840adea2f14a0d6d60`  
		Last Modified: Wed, 11 Dec 2019 18:20:30 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
