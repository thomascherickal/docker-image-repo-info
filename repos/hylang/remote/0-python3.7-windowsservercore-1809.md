## `hylang:0-python3.7-windowsservercore-1809`

```console
$ docker pull hylang@sha256:e9bc4cb3b267bfca32ff04fe0de04aa31b33d998252aa47f36513439be8d465f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `hylang:0-python3.7-windowsservercore-1809` - windows version 10.0.17763.1518; amd64

```console
$ docker pull hylang@sha256:53cef81b2687ae11a1f553e40e42c933d93b031d35edf6b0d560551fc5408081
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2445716207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e419e5a5a18d813b490455b5a37177369da04c9426dbb4d25426f2403c3908a`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 30 Oct 2020 00:18:21 GMT
ENV PYTHONIOENCODING=UTF-8
# Fri, 30 Oct 2020 00:38:21 GMT
ENV PYTHON_VERSION=3.7.9
# Fri, 30 Oct 2020 00:38:22 GMT
ENV PYTHON_RELEASE=3.7.9
# Fri, 30 Oct 2020 00:39:55 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Fri, 30 Oct 2020 00:39:57 GMT
ENV PYTHON_PIP_VERSION=20.2.4
# Tue, 03 Nov 2020 21:25:35 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/fa7dc83944936bf09a0e4cb5d5ec852c0d256599/get-pip.py
# Tue, 03 Nov 2020 21:25:36 GMT
ENV PYTHON_GET_PIP_SHA256=6e0bb0a2c2533361d7f297ed547237caf1b7507f197835974c0dd7eba998c53c
# Tue, 03 Nov 2020 21:26:22 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Tue, 03 Nov 2020 21:26:23 GMT
CMD ["python"]
# Tue, 03 Nov 2020 21:50:31 GMT
ENV HY_VERSION=0.19.0
# Tue, 03 Nov 2020 21:51:04 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Tue, 03 Nov 2020 21:51:05 GMT
CMD ["hy"]
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
	-	`sha256:cb794c56bcd1cabc090769fa40a9a01dc0b440ce7fd0dfbd8d3e17dab67ebd04`  
		Last Modified: Fri, 30 Oct 2020 00:43:41 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d93c270b62c46e0c90cb7c65946d56eaca48ec2dd27a962d12c93d302f557122`  
		Last Modified: Fri, 30 Oct 2020 00:51:21 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58685da8a57b5ecb6e9e67ff585bfeef48f213f2ed8d46c30a4afcc47d8b20d5`  
		Last Modified: Fri, 30 Oct 2020 00:51:22 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6080f4dc745368b145e4f003d86751713a8738e631374b06713396a413b5af01`  
		Last Modified: Fri, 30 Oct 2020 00:51:31 GMT  
		Size: 55.8 MB (55834750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aeb568993913fdb23b88750ab459832c9ba15cc49cc0ec125d08875f43927ce`  
		Last Modified: Fri, 30 Oct 2020 00:51:19 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a20197ba00f66d90b1c9173becf609429215481f93a85eb75ff7ab23c1c8926c`  
		Last Modified: Tue, 03 Nov 2020 21:30:22 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec80ff112c2d244af909ea0a4593681e159115f39c2f6b1b023fd294c65f7327`  
		Last Modified: Tue, 03 Nov 2020 21:30:21 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e443fd2fdd579b11a9dd33aef1594fd1cf2ec546e111d77cb0f5dc63f22723`  
		Last Modified: Tue, 03 Nov 2020 21:30:24 GMT  
		Size: 10.3 MB (10251144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc52745f13617a95758bfa710f529479cffcd3a9813edd1dca231d28f1708ed`  
		Last Modified: Tue, 03 Nov 2020 21:30:22 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e4abb794bf9416798110d064dbb1db18b61ec74983355a359083971d95ebf2e`  
		Last Modified: Tue, 03 Nov 2020 21:57:06 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fc35888512dea7a9060170346fc09e5de1e8e06f57a4afa54f7b3c1fec1806`  
		Last Modified: Tue, 03 Nov 2020 21:57:07 GMT  
		Size: 5.5 MB (5528864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecff1ba7a4a878a0bc1c06975f58b8e20a5eb08d08f9246e4e9be92afc7e9c14`  
		Last Modified: Tue, 03 Nov 2020 21:57:05 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
