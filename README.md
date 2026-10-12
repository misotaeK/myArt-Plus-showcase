# myArt+

A retro, Y2K-styled community site for artists: share artwork, talk in forums, form groups, host events and trade commissions.

**Live site: https://myartplus.site.je**

| Light theme | Dark theme |
|---|---|
| ![Sign-up page, light theme](assets/signup-light.jpg) | ![Sign-up page, dark theme](assets/signup-dark.jpg) |

## What it does

- **Profiles and artwork:** upload art by category (with credit for non-original work), commission status and price list, comments on profiles.
- **Forum:** boards, threads, replies, pinning and locking, search.
- **Groups:** create and join groups, admin approval, group chat with file sharing.
- **Direct messages:** friend requests, one-to-one chat with attachments, unread badges.
- **Exchange:** a board for offering and requesting art trades and commissions.
- **Events:** event pages with posters, RSVPs and comments; past events are cleaned up automatically.
- **Admin panel:** moderate users, review reports, approve groups.
- **Bilingual and themeable:** English and Turkish, light and dark theme.

## Built with

PHP 8 and MySQL (no framework), jQuery for the AJAX parts, hand-written CSS in a Y2K / early-web style. Hosted on a free shared host (InfinityFree).

## Security work

- CSRF tokens on every state-changing request, prepared statements everywhere, output escaping.
- Hardened sessions, rate limiting on login, sign-up and password reset.
- E-mail verification (HTML mail sent through Brevo's HTTPS API) and Cloudflare Turnstile captcha.
- Uploads are type-checked, renamed to safe names, and deleted from disk when replaced or when an account is removed.
- Secrets live outside the repository.

## Source code

The code is in a private repository. If you would like to read it, say hello on my GitHub profile and I will happily add you.
