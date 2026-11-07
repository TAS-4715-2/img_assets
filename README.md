# img_assets

Preview images for my **Steam Workshop** item pages — that is the whole purpose of
this repository.

## Why it exists

Steam renders images inside a Workshop description with `crossorigin="anonymous"`,
so the image host must answer with an `Access-Control-Allow-Origin` header. Ordinary
image hosts (imgbox, forum attachments, most CDNs) do not send it, which shows up as
a page full of broken images even though the links open fine. A small public GitHub
repository served through jsDelivr satisfies that requirement, costs nothing, and
needs no third-party image host account.

## It is not a general-purpose image host

- No upload endpoint, no API, no CI, no GitHub Pages, no Actions, no releases.
- No third-party content. Everything here is my own screenshots of my own mod pages.
- The entire repository is a handful of PNGs — a few megabytes in total.
- Nothing here is offered for reuse, hotlinking by others, or redistribution.

## What is hosted

| Folder | Used by |
|---|---|
| `va11halla/` | [VA-11 Hall-A Bartending Fan MOD](https://steamcommunity.com/sharedfiles/filedetails/?id=3831732004) — Workshop description screenshots (6 images) |

Referenced as:

```
https://testingcf.jsdelivr.net/gh/TAS-4715-2/img_assets@main/va11halla/01-preview-slogan-banner.png
```

`testingcf.jsdelivr.net` is used instead of the default `cdn.jsdelivr.net` because the
default entry point is unreachable from mainland China. It is the same jsDelivr
service on a different edge; the repository content is identical.

## Steam Workshop pages

- **VA-11 Hall-A Bartending Fan MOD** (Probably Stolen) —
  https://steamcommunity.com/sharedfiles/filedetails/?id=3831732004
- **VA-11 Hall-A Cassette** (companion music mod) —
  https://steamcommunity.com/sharedfiles/filedetails/?id=3831771576

## Copyright and takedown

All screenshots are in-game captures of *VA-11 Hall-A*, used to illustrate a
non-commercial fan mod. Characters, artwork and music belong to **Sukeban Games** and
their respective rights holders. No asset is redistributed as a standalone file and
no asset here is licensed for reuse.

If you are a rights holder and want an image removed, leave a comment on the
corresponding Workshop page and it will be deleted.

---

## 中文说明

本仓库**只**用于给本人发布在 Steam 创意工坊的 MOD 页面存放说明图，除此之外没有别的用途。

**为什么需要它**：Steam 渲染工坊简介里的图片时会带上 `crossorigin="anonymous"`，图床必须返回
`Access-Control-Allow-Origin` 头才显示得出来。普通图床（imgbox、论坛附件、多数 CDN）不返回这个头，
表现就是「链接能打开、页面上全是破图」。一个很小的 GitHub 公开仓 + jsDelivr 就能满足，不必再注册第三方图床。

**它不是通用图床**：

- 没有上传入口、没有 API、没有 CI、没有 GitHub Pages、没有 Actions、没有 releases；
- 不托管任何第三方内容，全部内容就是我自己 MOD 的几张游戏截图；
- 整个仓库只有几张 PNG，合计几 MB；
- 不对外提供外链、不复用、不授权他人二次使用。

| 目录 | 用途 |
|---|---|
| `va11halla/` | [VA-11 Hall-A 同人 MOD](https://steamcommunity.com/sharedfiles/filedetails/?id=3831732004) 的工坊简介配图（6 张） |

`testingcf.jsdelivr.net` 是 jsDelivr 的备用入口：默认的 `cdn.jsdelivr.net` 在中国大陆不可达，
两者是同一服务、不同节点，内容完全一致。

**相关工坊页面**：

- 调酒 MOD：https://steamcommunity.com/sharedfiles/filedetails/?id=3831732004
- 磁带 MOD（联动作品）：https://steamcommunity.com/sharedfiles/filedetails/?id=3831771576

**版权**：截图为《VA-11 Hall-A》游戏内画面，用于非盈利同人 MOD 的说明。角色、美术与音乐版权归
**Sukeban Games** 及相应权利人所有。这里不单独分发素材，也不授权任何人二次使用。
如有权利人希望移除某张图，在对应工坊页面留言即可，我会删除。
