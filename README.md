# DUSTLINE App Development Division / GitHub Pages

This folder is a static GitHub Pages site for the DUSTLINE app development division.

## Intended URL

`https://apps.dustline.jp/`

The root domain `https://dustline.jp/` should remain the magazine / sales website.

## GitHub Pages Setup

1. Create a GitHub repository, for example `dustline-app-development`.
2. Upload all files in this folder to the repository root.
3. In GitHub, open Settings -> Pages.
4. Set source to the default branch root.
5. Set custom domain to `apps.dustline.jp`.
6. In DNS, add a CNAME record:

```text
apps CNAME yuishoukai-ctrl.github.io
```

7. Enable HTTPS after DNS validation completes.

## Existing DUST LINE Website Change

Do not restructure the magazine website. Add only one link block to the existing Company page:

```html
<div class="company-profile-item company-profile-item--app-division">
  <dt>関連事業</dt>
  <dd>
    <a href="https://apps.dustline.jp/" rel="noopener">DUSTLINE アプリ開発事業部</a><br />
    <span>iOS / Androidアプリの企画・開発・運用、アプリ利用者向けサポート</span>
  </dd>
</div>
```

Recommended location: inside the current `COMPANY PROFILE / 事業者情報` block, near `事業内容` or `URL`.

## Apple Developer Program Note

Apple organization enrollment requires the legal entity name to match the D-U-N-S profile. DUSTLINE is represented on
this site as an operating name / app development division. Use the exact D-U-N-S legal entity name in Apple enrollment.

## Replace Before Public Use

- Confirm `support@dustline.jp` exists.
- Confirm `apps@dustline.jp` exists, or replace it with the actual domain email.
- Confirm the Apple Account email is associated with the same domain.
- Confirm D-U-N-S legal entity name, address, and phone match the Apple enrollment form.
