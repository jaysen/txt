---
category: Project
---

# SnapCipher (Concept Phase)

see the placeholder git repo here: https://github.com/jaysen/SnapCipher

**SnapCipher** is planned as a tool for encoding and decoding secret messages using photos of abstract or scrambled images—no access to the original file required. Designed for physical and digital use, it enables secure, offline visual communication with just a smartphone and a key.

#idea #dev #project #compsci

---

## 🔍 What Is SnapCipher?

SnapCipher transforms a message into a scrambled, abstract image that reveals its content only when decoded with the correct key. Unlike traditional steganography, the image doesn't look normal—it looks like noise, making it harder to detect and reverse-engineer.

- **Photograph-Based:** Snap a picture of a printed, drawn, or digital image to decode.
- **Key-Based Security:** Only someone with the right key can recover the message.
- **Offline & Resilient:** Works even with low-res, rotated, or imperfect captures.

---

## 🎯 Core Functionality (Planned)

- **Encode:** Convert a message into a scrambled visual pattern using a secret key.
- **Decode:** Recover the original message from a photo of the scrambled image.
- **No File Dependency:** Works from a photo of any medium—paper, screen, object.
- **Robust Tolerance:** Built to handle real-world distortions like angle and lighting.

---

## 🧠 Algorithm Goals

- Begin with QR codes with encrypted text.
- Next implement **black-and-white encoding** to simplify initial tests.
- Use **relative pixel positions** and **binary dot patterns** for data encoding.
- Apply **pseudo-random transformations** seeded by a user-provided key.
- Integrate **error correction** and **redundancy** for resilience.

---

## 🌐 Use Cases

- Private messaging through printed visuals
- Protest or activist communication via street posters or graffiti
- Physical access tokens and ARG puzzles
- Anonymous tagging in zines, clothing, or urban art

---

## 📦 Project Status

> 🚧 **Concept Phase**  
This project is currently in early planning and prototyping. The focus is on:
- Designing a reliable, portable encoding algorithm
- Building proof-of-concept tools for desktop and mobile
- Testing resilience with real-world inputs

---

## 💡 Roadmap

- [ ] Minimal encoder/decoder CLI tool
- [ ] Mobile prototype for photo decoding
- [ ] Visual design for QR-like scrambled patterns
- [ ] Testing tolerance to skew, blur, and lighting
- [ ] Documentation and community feedback loop

---

## 🔒 License

This project is licensed under the [GNU General Public License v3.0 (GPL-3.0)](https://www.gnu.org/licenses/gpl-3.0.en.html).  
We believe in user empowerment through open, auditable privacy tools.

---

## 🤝 Contributing

We're seeking collaborators with interest or expertise in:

- Image processing or CV (OpenCV, etc.)
- Cryptography / security tooling
- Mobile AR / camera frameworks
- Visual pattern design
- Radical or activist tech

Feel free to open an issue or discussion to join the project early.

---

## 📸 Example (Coming Soon)

We will include test images and decoding walkthroughs once the core logic is functional.

---

## 🗝️ Summary

**SnapCipher** makes it easy to send secure, physical-world messages using just images and a key. Take a picture, decode the cipher. No metadata. No trace. No file needed. Just light, ink, and trust.
