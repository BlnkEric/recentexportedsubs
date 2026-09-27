# recentexportedsubs

Auto-generated VPN subscription exports, published by `~/telegram-neko-sync`
(the v2sync pipeline). **Do not edit by hand** — files are overwritten on every
export run.

Add any link below as a *subscription* in *v2rayN* (desktop), *v2rayNG*
(Android) or *V2box* (iOS).

| group | what it is | subscription URL |
|---|---|---|
| **Export** | everything currently passing the health check | https://raw.githubusercontent.com/BlnkEric/recentexportedsubs/main/Export.txt |
| GitActive | 15 active channels mined from barry-far/v2ray-config | https://raw.githubusercontent.com/BlnkEric/recentexportedsubs/main/GitActive.txt |
| Daily | latest `bin.mudfish.net` payload from @DailyV2RY (replaced daily) | https://raw.githubusercontent.com/BlnkEric/recentexportedsubs/main/Daily.txt |
| Argo | @ARGO_VPNN file via ARGOO1_BOT | https://raw.githubusercontent.com/BlnkEric/recentexportedsubs/main/Argo.txt |
| Alpha | @V2ray_Alpha | https://raw.githubusercontent.com/BlnkEric/recentexportedsubs/main/Alpha.txt |
| VitoreNet | @filembad | https://raw.githubusercontent.com/BlnkEric/recentexportedsubs/main/VitoreNet.txt |
| ConfHub | @ConfigsHUB, 30-minute polling, dead nodes removed | https://raw.githubusercontent.com/BlnkEric/recentexportedsubs/main/ConfHub.txt |

Every file is a base64 body (the standard subscription format) preceded by
`#profile-title:` / `#support-url:` comment lines.

`index.json` records when each file was generated and how many nodes it holds.

The `.plain.txt` twins are not published — they only exist locally for
debugging.

## CI

`.github/workflows/publish-subs.yml` rebuilds the Pages index on every push to
`main` that touches `subs/**`. Enable it once:
**Settings → Pages → Source: GitHub Actions**, then the same files are also
served from `https://blnkeric.github.io/recentexportedsubs/`.
