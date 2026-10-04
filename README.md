# Recoditing

Montage vidéo et compositing dans une application native Rust/egui, avec rendu GPU Vulkan/DX12.

## Téléchargements

| Plateforme | Version publiée | Télécharger |
|---|---|---|
| **Windows x86_64** | 10.3.2 | [Installeur et fichiers Windows](https://github.com/Expected333/recoditing-releases/releases/tag/v10.3.2) |
| **Linux x86_64 — CachyOS / Arch** | 10.10.0 | [Archive Linux](https://github.com/Expected333/recoditing-releases/releases/tag/v10.10.0-linux) |

### Linux : extraire, lancer

Extraire `recoditing-10.10.0-linux-x86_64.tar.gz`, ouvrir le dossier extrait dans un terminal :

```bash
./recoditing
```

Binaire natif optimisé, sans Wine ni Docker. Il utilise les bibliothèques système : **FFmpeg 9**, ALSA, X11/Wayland, libxkbcommon, fontconfig, Vulkan et un pilote graphique adapté. Les dialogues de fichiers utilisent xdg-desktop-portal et le backend du bureau. Ce n'est pas une AppImage universelle ; les autres distributions ne sont pas validées.

Validation : **1 032 tests réussis**, import/export H.264 avec audio AAC, sauvegarde/réouverture des projets, lancement sur **RTX 3080 / Vulkan et NVDEC**. Détails et limites dans les notes de la release. SHA-256 fourni avec l'archive.

### Windows : canal habituel conservé

La publication Linux ne remplace aucun installeur, patch, signature ou manifeste Windows. La release marquée **Latest** reste celle du canal Windows pour préserver ses mises à jour automatiques. Aucun nouveau binaire Windows n'est annoncé par cette publication Linux.

## À savoir

Whisper et ses modèles doivent être configurés séparément pour la transcription. Les fonctions en ligne nécessitent leurs services. Les médias restent externes aux projets ; relocaliser les chemins lors d'un transfert Windows/Linux.
