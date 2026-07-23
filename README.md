# ADAPTIVE-MULTIMODAL-STEGANOGRAPHYFORSECURING-MEDICALHEALTHDATA
Medical data, including patient records, reports, images, and multimedia
content, contains highly sensitive information that requires secure storage and
transmission. While cryptographic techniques ensure confidentiality, the presence of
encrypted data may still reveal sensitive information. Steganography addresses this by
hiding data within multimedia carriers, but traditional single-modal approaches lack
robustness and flexibility. Additionally, medical data is heterogeneous, consisting of
text, images, and audio, making single-modal methods less effective. This project
proposes an adaptive multimodal steganography approach to securely embed medical
data across multiple carriers, improving security, imperceptibility, and robustness.
This project proposes an adaptive multimodal steganography framework
to enhance the security of sensitive medical data by utilizing multiple multimedia
carriers. The system supports various embedding techniques, including text-in-audio,
text-in-video, image-in-image, and audio-in-image, allowing different types of medical
information to be embedded into the most suitable carrier modality. By intelligently
mapping each data type to an appropriate medium, the framework ensures efficient
utilization of carrier capacity while preserving the visual and perceptual quality of
the cover media. Unlike traditional single-modal approaches, the proposed multimodal
strategy distributes secret data across multiple carriers, reducing payload concentration
and minimizing the risk of detection and steganalysis attacks. At the receiver end,
the system enables accurate extraction and reconstruction of the original medical data,
ensuring data integrity and reliability. Experimental evaluation demonstrates that the
proposed system achieves approximately 95% data recovery while maintaining high
imperceptibility and robustness against common distortions, making it a secure and
efficient solution for safeguarding healthcare information.

The system supports secure embedding of:
- Text into Audio
- Text into Video
- Image into Image
- Audio into Image

A decision engine dynamically routes each data modality to the most appropriate embedding module, enabling efficient and reliable multimodal communication.

---

## Features

- Adaptive decision engine for intelligent carrier selection
- Image-in-Image steganography using LiDiNet
- Text-in-Video steganography with VAE, MFICF, STC, and LSB embedding
- Text-in-Audio steganography using HIFI-Stego
- Audio-in-Image steganography using STFT and LSB
- High-quality reconstruction of hidden data
- Streamlit-based interactive user interface
- Secure multimodal data transmission

---

## System Architecture

The framework consists of the following stages:

1. Secret Data Preprocessing
2. Adaptive Decision Engine
3. Carrier Media Selection
4. Multimodal Steganography Modules
5. Stego Media Generation
6. Data Extraction and Reconstruction

---

## Technologies Used

- Python
- Streamlit
- PyTorch
- TensorFlow / Keras
- OpenCV
- NumPy
- SciPy
- Librosa
- ImageIO
- FFmpeg

---

## Performance

| Module | Performance |
|--------|-------------|
| Image-in-Image | PSNR > 42 dB, SSIM > 0.995 |
| Audio-in-Image | PSNR ≈ 45 dB, SSIM > 0.993 |
| Text-in-Video | Capacity up to 20,000 characters |
| Text-in-Audio | SNR ≈ 48.5 dB, PESQ > 4.5 |

The proposed framework achieves high imperceptibility, reliable data recovery, and efficient multimodal embedding while maintaining media quality.

---

## Applications

- Secure Medical Data Transmission
- Electronic Health Records (EHR)
- Telemedicine
- Healthcare Cloud Storage
- Secure Multimedia Communication
- Digital Forensics

---

## Future Enhancements

- Real-time multimedia streaming
- Cloud-based deployment
- Additional carrier modalities
- AI-based adaptive carrier optimization
- Enhanced robustness against steganalysis attacks
