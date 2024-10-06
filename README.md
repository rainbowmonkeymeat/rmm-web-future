# rmm-sites
Rainbow Monkey Meat Static Sites

Hugo driven, hosted on Cloudflare pages

## Preview in coder (and potentially codespaces) environment

Heavily based on name of container - may need to share out initially, then adjust from ports page

```sh
hugo serve -D --port 1314 --baseURL="https://1314--main--acctadminsuite--ssmiller25.coder.r15cookie.com/" --appendPort=false
```

## Code Snippets - Modules

WARNING: Does not work, as this theme is not bundled as a go module (I think...)

```sh
curl -LO https://github.com/gohugoio/hugo/releases/download/v0.121.1/hugo_0.121.1_linux-amd64.deb
sudo dpkg -i hugo*deb
sudo apt install hugo
sudo apt install golang
hugo new site rmm-future --format yaml
cd rmm-future

git submodule add --depth=1 https://github.com/felicianotech/hugo-theme-lean-launch-page.git rmm-future/themes/lean-launch-page
cd rmm-future/themes/lean-launch-page
git pull
```

Updated

```sh
git submodule update --remote --merge
```
