We use a subset of Marianne font because we know we use just a few characters for our list. This
shrinks the font file size noticeably!

Example command to use to generate the subset with glyphhanger:

```
glyphhanger \
  --subset="./Marianne-Regular.woff2" \
  --formats=woff2 \
  --whitelist="DeskLaSuiteNumériqueMessagerieTchapResanaFranceTransfertContactsGristLePadWebConférencedel'ÉtatWebinaire  "
```

## ⚠

Make sure to also update the `unicode-range` on the `@font-face` CSS rule. You can get it on the
glyphhanger command output.

Assuming you have the Marianne-Regular.woff2 file (you can take it from the DSFR).
