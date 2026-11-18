# video-thumbnail-sizes

An open reference of thumbnail and cover image sizes for YouTube, YouTube Shorts, TikTok, Instagram Reels and Facebook, with a link to the official source for every number.

Many "official sizes" published online are really conventions. This reference marks each value as:

- **documented**: stated by the platform in its help center or developer docs
- **convention**: common practice, not an official requirement

Last verified: **2026-11-16**. Machine-readable data: [`sizes.json`](sizes.json).

## Quick reference

| Placement | Prepare | Ratio | Notes |
|---|---|---|---|
| YouTube video | 3840×2160 (min. 640 wide) | 16:9 | JPG or PNG; 2 MB on mobile, 50 MB on a computer |
| YouTube Shorts | 2160×3840 (min. 640 high) | 9:16 | Added in YouTube Studio on a computer |
| TikTok cover | A frame of your 9:16 video | 9:16 | No official image spec; 1080×1920 is a convention |
| Instagram Reels cover | 9:16, e.g. 1080×1920 | 9:16 | JPEG up to 8 MB via API; feed crops to 1:1 |
| Facebook video / Reels | Match the video, e.g. 1080×1920 | Same as video | Thumbnail up to 10 MB via API |

## YouTube generated thumbnail sizes

After upload, YouTube serves fixed-size copies at `https://i.ytimg.com/vi/<VIDEO_ID>/<name>.jpg`:

| Name | Size | Always available |
|---|---|---|
| `default` | 120×90 | yes |
| `mqdefault` | 320×180 | yes |
| `hqdefault` | 480×360 | yes |
| `sddefault` | 640×480 | no |
| `maxresdefault` | 1280×720 | no |

## Sources

- YouTube Help: Add custom thumbnails — https://support.google.com/youtube/answer/72431
- YouTube Data API: Thumbnails — https://developers.google.com/youtube/v3/docs/thumbnails
- TikTok Support: Adding a video cover — https://www.tiktok.com/support/faq_detail?id=7636670084584479253&category=web_account
- TikTok ads video specifications — https://ads.tiktok.com/help/article/video-ads-specifications?lang=en
- Instagram Help: Reels resolution and size — https://help.instagram.com/1038071743007909
- Meta for Developers: IG User Media — https://developers.facebook.com/docs/instagram-platform/instagram-graph-api/reference/ig-user/media
- Meta for Developers: Reels Publishing API — https://developers.facebook.com/docs/video-api/guides/reels-publishing/
- Meta for Developers: Video Thumbnails — https://developers.facebook.com/docs/graph-api/reference/video/thumbnails/

A longer explanation with examples is available on [ThumbnailFetch](https://thumbnailfetch.com/en/blog/thumbnail-sizes-all-platforms).

## Contributing

Platform specs change. If a value is outdated, open an issue with a link to the official source.

## License

[MIT](LICENSE) © Avadalabs
