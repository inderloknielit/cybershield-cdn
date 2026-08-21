# CyberShield Content Delivery Network (CDN)

This repository serves as the official, secure Content Delivery Network for the **CyberShield** mobile application. It is managed by **NIELIT** to provide real-time Over-The-Air (OTA) updates to the curriculum without requiring a full app re-installation.

## 📁 Repository Structure

- `/ota/version.json`: Contains the current content version number. The app checks this file on every launch.
- `/ota/units.json`: The "Master Map" of the curriculum. Contains all Units, Modules, Lessons, and Quiz questions.
- `/ota/images/`: A directory hosting all visual diagrams and illustrations used inside the flashcards.

## 🚀 How to Push Updates

1. **Update Content**: Modify `units.json` with new lessons or quiz questions.
2. **Update Version**: Increment the `latest_content_version` number in `version.json`.
3. **Commit & Push**: Once pushed to the `master` branch, all active CyberShield users will receive the update within minutes.

## 🛡️ Security Guidelines
- **Integrity**: Ensure the JSON structure remains valid before pushing. An invalid JSON will prevent users from receiving updates.
- **Privacy**: No user-identifiable information should ever be pushed to this public repository.
- **Optimized Assets**: Ensure all images in `/images` are compressed PNGs to save user bandwidth.

---
Managed by **NIELIT (National Institute of Electronics & Information Technology)**, India.
