<div align="center">
  <p><img src=".github/assets/icon.svg" align="center" width="128"/></p>
  <h1>LOGOBASE</h1>
</div>

<table><tr><td align="center" width="9999">
  &nbsp;<p>Technology logo pack intended for very seamless integration into README.md files or visual assets such as LinkedIn banners, provided in both dark and light variants for optimal flexibility and consistency.</p>&nbsp;
</td></tr></table>

### Logo Collection

<!-- START_TABLE -->
<!-- CEASE_TABLE -->

### Create Markdown Banner

#### 1. Banner Preview

<table><tr><td align="center" height="72" width="9999">
  <picture><source media="(prefers-color-scheme: dark)" srcset="logos/horizontal-dark.png"><img src="logos/horizontal-light.png" align="center" width="48"/></picture>
  <picture><source media="(prefers-color-scheme: dark)" srcset="logos/circle-dark.png"><img src="logos/circle-light.png" align="center" width="48"/></picture>
  <picture><source media="(prefers-color-scheme: dark)" srcset="logos/vertical-dark.png"><img src="logos/vertical-light.png" align="center" width="48"/></picture>
  <picture><source media="(prefers-color-scheme: dark)" srcset="logos/square-dark.png"><img src="logos/square-light.png" align="center" width="48"/></picture>
  <picture><source media="(prefers-color-scheme: dark)" srcset="logos/horizontal-dark.png"><img src="logos/horizontal-light.png" align="center" width="48"/></picture>
</td></tr></table>

#### 2. Gather the Logos

```shell
deposit="images" && mkdir -p "$deposit"
baseurl="https://github.com/olankens/logobase/raw/HEAD/logos"
for f in {circle,horizontal,square,vertical}-{dark,light}; do
  curl -Lo "$deposit/$f.png" "$baseurl/$f.png"
done
```

#### 3. Create the Banner

```md
<table><tr><td align="center" height="72" width="9999">
  <picture><source media="(prefers-color-scheme: dark)" srcset="images/horizontal-dark.png"><img src="images/horizontal-light.png" align="center" width="48"/></picture>
  <picture><source media="(prefers-color-scheme: dark)" srcset="images/circle-dark.png"><img src="images/circle-light.png" align="center" width="48"/></picture>
  <picture><source media="(prefers-color-scheme: dark)" srcset="images/vertical-dark.png"><img src="images/vertical-light.png" align="center" width="48"/></picture>
  <picture><source media="(prefers-color-scheme: dark)" srcset="images/square-dark.png"><img src="images/square-light.png" align="center" width="48"/></picture>
  <picture><source media="(prefers-color-scheme: dark)" srcset="images/horizontal-dark.png"><img src="images/horizontal-light.png" align="center" width="48"/></picture>
</td></tr></table>
```
