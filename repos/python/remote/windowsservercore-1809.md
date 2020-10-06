## `python:windowsservercore-1809`

```console
$ docker pull python@sha256:3c19207330844b341e117b5e22bddf372321958e235700aafae383235f272dab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `python:windowsservercore-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull python@sha256:3018fd74f471bb788fe917c71ef99518bf9128e4942fe1d98ddcc58c9f2aa741
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2421603229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8990ffad340d53161413458a7cea920599a173dd5ace35528f32220e95c3406b`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 06 Oct 2020 21:19:24 GMT
ENV PYTHON_VERSION=3.9.0
# Tue, 06 Oct 2020 21:19:25 GMT
ENV PYTHON_RELEASE=3.9.0
# Tue, 06 Oct 2020 21:21:14 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Tue, 06 Oct 2020 21:21:15 GMT
ENV PYTHON_PIP_VERSION=20.2.3
# Tue, 06 Oct 2020 21:21:16 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Tue, 06 Oct 2020 21:21:17 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Tue, 06 Oct 2020 21:22:01 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Tue, 06 Oct 2020 21:22:02 GMT
CMD ["python"]
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
	-	`sha256:0ccd08b9a3b1df9994da1ba85dceaa8ad45c85e81b9dfcf3b622f3065c41c59c`  
		Last Modified: Tue, 06 Oct 2020 21:23:40 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d7ed4ae8f8169fc88fbc2bd0dec7cd25ff751b1e824c3935ac992d57c50d11`  
		Last Modified: Tue, 06 Oct 2020 21:23:39 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe232c848495ba40261d1fa4b4f08f9db48e732c1055136c5d32cfd0f0deeb7`  
		Last Modified: Tue, 06 Oct 2020 21:23:50 GMT  
		Size: 60.0 MB (60027360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41ea40f3bfd734d7c431367dc000e3d33ecdd1b7ef2d6b05bed6949eda8e778`  
		Last Modified: Tue, 06 Oct 2020 21:23:37 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624ae53d2d8e6b9268eac41b5bf3d1ec4335fe13dd73228b161a50553789d75e`  
		Last Modified: Tue, 06 Oct 2020 21:23:37 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e069583c0f0650b1123bd875c349d3b0a95a81fd62755a6a370d78a1370d173`  
		Last Modified: Tue, 06 Oct 2020 21:23:37 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493c4878b1678bc50a16c2901103650c465ce0c973d48dfe6fe2e54daacac3a8`  
		Last Modified: Tue, 06 Oct 2020 21:23:40 GMT  
		Size: 10.3 MB (10295674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a092fe419e82a9872d74a4fa6f694c540c202c0348475c248782ccea7031a4d8`  
		Last Modified: Tue, 06 Oct 2020 21:23:37 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
