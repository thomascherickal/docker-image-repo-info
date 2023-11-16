## `pypy:3-windowsservercore-1809`

```console
$ docker pull pypy@sha256:716b07d1872edb42fc31dde6287b156e01e30ed9bc3d68f34b62730d8a6aa44e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `pypy:3-windowsservercore-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull pypy@sha256:45c7532e5a6596beee450c9f9c6a9b08b4f664c30f12071b20893a7bf5c137f7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2103243619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ed3b148b47f7f4905bb8cd7d8dd4cf790c894cc1d348d0eec42bd454560ae59`
-	Default Command: `["pypy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Thu, 09 Nov 2023 17:56:40 GMT
RUN Install update 10.0.17763.5122
# Thu, 16 Nov 2023 01:37:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Nov 2023 07:46:44 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Thu, 16 Nov 2023 07:48:07 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x64.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = 'da66717784c192f1004e856bbcf7b3e13b7bf3ea45932c48e4c9b9a50ca80965'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Thu, 16 Nov 2023 07:48:08 GMT
ENV PYPY_VERSION=7.3.13
# Thu, 16 Nov 2023 07:49:54 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.10-v7.3.13-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = '5b99422fb8978b2f4bbf97961bca49963a82dc47c2fa51b7d23c493db3a2e0f0'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.10-v7.3.13-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy --version") ...'; 	pypy --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Thu, 16 Nov 2023 07:49:55 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 16 Nov 2023 07:49:56 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 16 Nov 2023 07:52:05 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$pipVersion = & pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)'; 	$setuptoolsVersion = & pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)'; 		Write-Host ('Installing "pip == {0}", "setuptools == {1}" ...' -f $pipVersion, $setuptoolsVersion); 	pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $pipVersion) 		('setuptools == {0}' -f $setuptoolsVersion) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Thu, 16 Nov 2023 07:52:06 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bb9e009deb881cb90e8b4318258e03882de9bc9b312b763654b59cd13d0bb`  
		Last Modified: Tue, 14 Nov 2023 19:53:30 GMT  
		Size: 406.8 MB (406811201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7a1cc914f0f5e059bfdf02906a6e052b1c97cebaf91eb6c2fd835cfddebda2`  
		Last Modified: Thu, 16 Nov 2023 02:26:46 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e430ddef0312e491229f8dfb31c1c4b5a4c5c2376b98a14535ce6c5a80ffb943`  
		Last Modified: Thu, 16 Nov 2023 08:54:59 GMT  
		Size: 438.1 KB (438076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5a86f421addaeba63d93e1af89aaeb9017a3ecc28ebdc0de7cb683e7349980`  
		Last Modified: Thu, 16 Nov 2023 08:55:02 GMT  
		Size: 15.4 MB (15437374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d52bc09e21e8ea36cdaf8bdf8228a3ba92b7b60d10a6705e89e33532615362`  
		Last Modified: Thu, 16 Nov 2023 08:54:58 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36070f329097c467ca7c995acfeeabe8328963d78fe0fcf385d0beee9ba636e4`  
		Last Modified: Thu, 16 Nov 2023 08:55:03 GMT  
		Size: 26.1 MB (26096439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c777ed6751299fc9eba701e0999e79a7b3b1d85edab553c15985e280e1a103e4`  
		Last Modified: Thu, 16 Nov 2023 08:54:56 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e7cb799409d734d8cc250e90a939e7a6844176af150cfd124399dc7cab98fe`  
		Last Modified: Thu, 16 Nov 2023 08:54:57 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18779e6b68f6df91ac675e8749b33a8a626a6389d85bd43fab653e1a2118cb02`  
		Last Modified: Thu, 16 Nov 2023 08:54:58 GMT  
		Size: 3.8 MB (3833122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49a8f9aeb4b448ed794fe34a7cb40bd7797b4da4ea35e9942632a3402f54d7c`  
		Last Modified: Thu, 16 Nov 2023 08:54:56 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
