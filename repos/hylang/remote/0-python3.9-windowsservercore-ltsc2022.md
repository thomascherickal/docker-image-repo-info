## `hylang:0-python3.9-windowsservercore-ltsc2022`

```console
$ docker pull hylang@sha256:0457d4ebd79e241c2f2ff439688cd28b036605f7a4340f68165bb815cc13ffe1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.825; amd64

### `hylang:0-python3.9-windowsservercore-ltsc2022` - windows version 10.0.20348.825; amd64

```console
$ docker pull hylang@sha256:f36846c3468bced7ea732ed95c3904b7a8d716b5ce15525fc62986ef0d958e82
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2360610316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75930453cf35bb2c43c516ff317c84a72e783e2d62e2ebfc2b72b4ca6786c89c`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Mon, 04 Jul 2022 17:46:55 GMT
RUN Install update 10.0.20348.825
# Tue, 12 Jul 2022 19:25:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 20:35:01 GMT
ENV PYTHONIOENCODING=UTF-8
# Tue, 12 Jul 2022 20:50:00 GMT
ENV PYTHON_VERSION=3.9.13
# Tue, 12 Jul 2022 20:51:18 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f ($env:PYTHON_VERSION -replace '[a-z]+[0-9]*$', ''), $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Tue, 12 Jul 2022 20:51:19 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Tue, 12 Jul 2022 20:51:20 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Tue, 26 Jul 2022 23:24:23 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/49ca29908cfd49683da12f2d5a4fa5689539f9d9/public/get-pip.py
# Tue, 26 Jul 2022 23:24:25 GMT
ENV PYTHON_GET_PIP_SHA256=d077d469ce4c0beaf9cc97b73f8164ad20e68e0519f14dd886ce35d053721501
# Tue, 26 Jul 2022 23:25:12 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$env:PYTHONDONTWRITEBYTECODE = '1'; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Tue, 26 Jul 2022 23:25:13 GMT
CMD ["python"]
# Tue, 26 Jul 2022 23:46:43 GMT
ENV HY_VERSION=0.24.0
# Tue, 26 Jul 2022 23:46:43 GMT
ENV HYRULE_VERSION=0.2
# Tue, 26 Jul 2022 23:47:41 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION) ('hyrule == {0}' -f $env:HYRULE_VERSION)
# Tue, 26 Jul 2022 23:47:42 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e1a27cb9d4615dec325f2cbabac4ca1f65413bdbb8b440cc961df032993a9b81`  
		Size: 863.4 MB (863367943 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6452cb934201756f0ed9fb5e0cbea54a22a66412cb696ff30a1923d456e28bcf`  
		Last Modified: Tue, 12 Jul 2022 20:20:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef330eb8cab3834d9737ff92915047264f01ac2d39da71a4aa5e63eddef3204`  
		Last Modified: Tue, 12 Jul 2022 20:56:31 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090ce0c092147a617936f3f964fb55f8bd2930749dc550642dbc5d65f33b8f6d`  
		Last Modified: Tue, 12 Jul 2022 20:57:58 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fca5498c8a0c78b9b210db675489ce5e7a2a843930d82da78dd23cda2dabea9`  
		Last Modified: Tue, 12 Jul 2022 20:58:05 GMT  
		Size: 52.0 MB (51982748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29619e5e28282b5438d24f3da90273aafb5b1e5630c96f3eaafe80a26ea770aa`  
		Last Modified: Tue, 12 Jul 2022 20:57:58 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc454d63f220b0999f197261db2a80c712afc3d327d9a6d80eb8f2a68e4da259`  
		Last Modified: Tue, 12 Jul 2022 20:57:56 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4642bebe9b8868af7b869a35f52a2bd142277d1a8fb8104a2fec55e903c91f4`  
		Last Modified: Tue, 26 Jul 2022 23:28:58 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe947ac947d6b969c49d05ad245fb85d5328648483a16007b0aa96d538da861`  
		Last Modified: Tue, 26 Jul 2022 23:28:58 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46098b1a16b09dd582fb2ad98e610dc2cfbb6ccd250243b6d8470bd5d6b92995`  
		Last Modified: Tue, 26 Jul 2022 23:29:00 GMT  
		Size: 3.7 MB (3739540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638ae9e17659b3d741ef8135a6426c095c633eeb95774b907c40bbbd3525896d`  
		Last Modified: Tue, 26 Jul 2022 23:28:58 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4340f4c7cd5e246878812b41c64e660ee889ac0606fbbf860d343a8d1ea9afc`  
		Last Modified: Wed, 27 Jul 2022 12:04:43 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54e2fb14b1fdc4f287a432f78491d06e9ac8fd44e5919da8694117a9bca5bd7`  
		Last Modified: Wed, 27 Jul 2022 12:04:43 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b394341d33fe69f238227f8a661dba59215fe837105c7dc42cfabb5015d451`  
		Last Modified: Wed, 27 Jul 2022 12:04:45 GMT  
		Size: 4.6 MB (4641343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964b54d29c5d74ec1590ba453b1a5fbfa590fb428a9ecd9d38edc37e332f7b4a`  
		Last Modified: Wed, 27 Jul 2022 12:04:43 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
