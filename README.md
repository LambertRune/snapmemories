# SnapMemories Downloader

Een 100% client-side Snapchat Memories downloader. Privacy-first, GDPR-compliant.

## 🛡️ Privacy & GDPR Compliance

Deze tool is **100% legaal** om te deployen en te delen omdat:

- **100% Client-Side**: Alle verwerking gebeurt in de browser van de gebruiker
- **Geen Data Opslag**: Wij slaan geen bestanden of persoonlijke gegevens op
- **Geen Data Transmissie**: Data gaat nooit naar onze servers
- **Geen Tracking**: Geen analytics, cookies of fingerprinting
- **Direct Download**: Bestanden gaan rechtstreeks van Snapchat naar de gebruiker

### GDPR Artikelen

| Artikel | Compliance |
|---------|------------|
| Art. 5 (Data Minimization) | ✅ Geen data verzameling |
| Art. 6 (Lawful Basis) | ✅ Gebruiker initieert zelf |
| Art. 17 (Right to Erasure) | ✅ N/A - geen data opslag |
| Art. 25 (Privacy by Design) | ✅ Client-side architectuur |

## 🚀 Deployment

### Lokaal testen

```bash
cd src && python3 -m http.server 8080
```

### Deploy naar Coolify

1. Push naar GitHub/GitLab
2. In Coolify: New Resource → Docker Compose
3. Voeg environment variable toe:
   - `CLOUDFLARE_TUNNEL_TOKEN` = je tunnel token
4. Deploy!

### Environment Variables (Coolify)

| Variable | Beschrijving |
|----------|--------------|
| `CLOUDFLARE_TUNNEL_TOKEN` | Je Cloudflare Tunnel token |

### Cloudflare Tunnel Token Krijgen

1. Ga naar [Cloudflare Zero Trust Dashboard](https://one.dash.cloudflare.com/)
2. Access → Tunnels → Create Tunnel
3. Kies "Cloudflared" en geef een naam
4. Kopieer de token
5. Voeg toe in Coolify als `CLOUDFLARE_TUNNEL_TOKEN`

## 📁 Project Structuur

```
snapmemories-app/
├── src/
│   └── index.html      # Complete app (single file)
├── nginx/
│   └── default.conf    # Nginx configuratie
├── Dockerfile          # Docker image
├── docker-compose.yml  # Coolify + Cloudflare Tunnel
└── README.md
```

## ⚖️ Legale Status

**Ja, dit is legaal om te deployen en te delen.**

Redenen:
1. De tool verwerkt geen data - alles blijft bij de gebruiker
2. Snapchat biedt zelf data export aan (GDPR recht)
3. Wij faciliteren alleen het organiseren van eigen data
4. Geen trademark inbreuk (we gebruiken geen Snapchat logo's)
5. Duidelijke disclaimer op de site

## 📄 Licentie

MIT License - Vrij te gebruiken en aan te passen.

---

Gemaakt door [Phiosk Development](https://development.phiosk.be)

