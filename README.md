# ac5_A4_codespaces

## Codespaces
[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/bartdorlandt/ac5_A4_codespaces)


## Docker test from avd sandbox
```bash
docker run --rm -it -v $(pwd):/home/avd/workspace -w /home/avd/workspace ghcr.io/bartdorlandt/ac5_a4_codespaces/my_container:latest zsh
```

```bash
docker run --rm -it -v $(pwd):/home/avd/workspace -w /home/avd/workspace ghcr.io/bartdorlandt/ac5_a4_codespaces/lab:uid-1009
```

```bash
docker run --rm -it --privileged --name lab --detach -w /lab -v /sandbox/lab_dir:/lab -v /var/lib/docker -e PASSWORD=labpass124 -p 5000:5000 ghcr.io/bartdorlandt/ac5_a4_codespaces/lab:uid-1009-rev0.1
```