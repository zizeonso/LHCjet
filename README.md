# LHCjet

## Code Overview

- **Data preprocessing**  
  Jet images are normalised and centre-cropped from 100×100 to 40×40 to reduce dimensionality while preserving the core energy deposition. Scalar high-level features are processed separately and aligned with image labels.

- **Model implementations**  
  Multiple neural architectures are implemented, including:
  - Image-only CNN models
  - Feature-only fully connected networks
  - Hybrid multi-input models combining images and scalar features
  - Extended architectures incorporating ECAL and HCAL image inputs

- **Training and evaluation**  
  Models are trained using supervised learning with cross-entropy loss and the Adam optimiser. Performance is evaluated using accuracy, F1 score, AUC, confusion matrices, and per-class ROC curves.

---

## Notes

- Large raw datasets are not included in this repository.
- The code is intended for research and educational purposes rather than production deployment.
- The structure is designed to allow easy extension to alternative architectures or additional input modalities.
- There is a data leak issue maybe in data preparation part

