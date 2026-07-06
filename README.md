# lawrence-claude-plugins

marketplace pribadi untuk plugin claude code — Lawrence Philemon.

## install

```bash
# 1. tambahkan marketplace (sekali saja)
/plugin marketplace add <username>/lawrence-claude-plugins

# 2. install plugin
/plugin install page-copy-architect@lawrence-plugins
```

atau via CLI di luar sesi:

```bash
claude plugin marketplace add <username>/lawrence-claude-plugins
claude plugin install page-copy-architect@lawrence-plugins
```

ganti `<username>` dengan username github kamu.

## plugins

| plugin | deskripsi |
|---|---|
| `page-copy-architect` | P.A.G.E framework — arsitektur product page yang menyeimbangkan SEO dan conversion copywriting via zone system |

## menambah plugin baru

1. buat folder baru di `plugins/<nama-plugin>/` dengan struktur:
   ```
   plugins/<nama-plugin>/
   ├── .claude-plugin/plugin.json
   └── skills/<nama-skill>/SKILL.md
   ```
2. daftarkan entry baru di `.claude-plugin/marketplace.json` (field `plugins`)
3. commit + push
4. di claude code: `/plugin marketplace update lawrence-plugins`

## update plugin yang sudah ada

edit file plugin → bump `version` di `plugin.json` dan `marketplace.json` → push → `/plugin marketplace update lawrence-plugins`.
