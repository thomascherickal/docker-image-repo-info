## `hylang:python3.9-windowsservercore-ltsc2022`

```console
$ docker pull hylang@sha256:1b6454b0f70fa25a33dfa5a9346cb74cb4ffc43404aa6fc14ddcda11976cc1e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.825; amd64

### `hylang:python3.9-windowsservercore-ltsc2022` - windows version 10.0.20348.825; amd64

```console
$ docker pull hylang@sha256:ab414f6abe47884b88d263fa194087b467e3754eabaab05e1734c820964fb0d1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2360613529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2edbc9f61f3cab129763a468befef9b6e1382a9892b420fff2b9dc709e845f46`
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
# Tue, 12 Jul 2022 20:51:21 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6ce3639da143c5d79b44f94b04080abf2531fd6e/public/get-pip.py
# Tue, 12 Jul 2022 20:51:22 GMT
ENV PYTHON_GET_PIP_SHA256=ba3ab8267d91fd41c58dbce08f76db99f747f716d85ce1865813842bb035524d
# Tue, 12 Jul 2022 20:52:11 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$env:PYTHONDONTWRITEBYTECODE = '1'; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Tue, 12 Jul 2022 20:52:12 GMT
CMD ["python"]
# Tue, 12 Jul 2022 21:14:34 GMT
ENV HY_VERSION=0.24.0
# Tue, 12 Jul 2022 21:14:35 GMT
ENV HYRULE_VERSION=0.2
# Tue, 12 Jul 2022 21:15:34 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION) ('hyrule == {0}' -f $env:HYRULE_VERSION)
# Tue, 12 Jul 2022 21:15:35 GMT
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
	-	`sha256:f52d69e25961c034eba0d412b6c4b582e4c9522286b4cb73fcb99b02ec007e63`  
		Last Modified: Tue, 12 Jul 2022 20:57:56 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c188b281f9d0832bd7074e2291ca3d93e0c0905ab280d79be1cbb25d652976`  
		Last Modified: Tue, 12 Jul 2022 20:57:56 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b024f75f10c9fd21b7ff94d77b20fe8f49f04c0a3cec4e41abb3fc5752434d1`  
		Last Modified: Tue, 12 Jul 2022 20:57:57 GMT  
		Size: 3.7 MB (3732419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f376394e3ed5e3d8457eeb4393b3dd9db081d21a3e7b8f59f5bcc0d5becd9009`  
		Last Modified: Tue, 12 Jul 2022 20:57:56 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ab472c7dc930db6ebe32660e0b527ddd8e43bdbdadef933b69ce1028d34218`  
		Last Modified: Tue, 12 Jul 2022 21:19:22 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994182feaa83f6a7bf15d140def2284981045fdb71a47e7ab99ab500c0850fbe`  
		Last Modified: Tue, 12 Jul 2022 21:19:23 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474b9372f90762e8a9b12ea46e2df2bcb2a41ea19b4d5205d6e2678cdef7a628`  
		Last Modified: Tue, 12 Jul 2022 21:19:24 GMT  
		Size: 4.7 MB (4651429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99387f6a7ade66d4e187b3d1ed3253ce57702f292e90ad613571d6401bd322b9`  
		Last Modified: Tue, 12 Jul 2022 21:19:22 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
