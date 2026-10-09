# Google Sheet layout

One Google Sheet with two tabs. Row 1 is the header row.

## Clients

One row per brand. `tag` is what goes at the start of the Telegram caption (e.g. `#aurelle`).

| tag | brand_name | tone | languages | audience |
|---|---|---|---|---|
| aurelle | Aurelle Jewellery | warm, elegant, gift-focused, not salesy | EN, AR | women 20-40 in the UAE |

## Content

Headers only. The workflow adds the rows.

| id | date | client_tag | photo_file_id | notes | caption_en | caption_ar | hashtags | status |
|---|---|---|---|---|---|---|---|---|

- `id` is the n8n execution ID, used to find the row again after approval.
- `photo_file_id` is Telegram's ID for the photo, so the image doesn't need to be stored.
- `status` is `drafted`, then `posted` or `rejected`.
