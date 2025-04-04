# 🗺️ Multimodal-Map-Search

**Multimodal-Map-Search** is an AI-powered search engine that enables users to explore large-scale map collections through **text-based** or **image-based** queries. Users can enter specific queries (like a country, city, or historical region) or upload a sample map image to retrieve visually and semantically similar map images.

This project leverages multimodal machine learning to enhance the discoverability of map data—useful in **education**, **research**, and **digital archives**.

---

## ✨ Key Features

-  **Text-based search**: Retrieve relevant maps by typing natural language queries (e.g., "ancient map of Rome").
-  **Image-based search**: Upload a map image to find visually similar maps.
-  **Multimodal AI**: Uses OpenAI's **CLIP** model to connect images and text in a shared embedding space.
-  **Fast & Scalable**: Searches are powered by precomputed embeddings for over half a million maps.
-  **Interactive UI**: Simple and intuitive interface built with **Gradio**.

---

##  Technologies Used

- **CLIP (Contrastive Language–Image Pretraining)** – for multimodal embeddings
- **PyTorch** – model backbone and inference
- **Transformers** – model handling
- **Gradio** – web-based user interface
- **Pillow** – image handling and preprocessing

---

## 🗂 Dataset & Embeddings

This project uses **precomputed embeddings** for a large collection of map images.

🔗 **Download the required files**:  
[📁 Google Drive Folder](https://drive.google.com/drive/folders/161PYWfSHI393Qh6RPJolPopAGvaMffMq?usp=sharing)

Files:
- `mapimg.pt`
- `mapimg_idx.pt`
- `mapimg_normalized.pt`

---

## 🚀 Getting Started

Follow these steps to run the project locally:

### 1. Clone the repository
```bash
git clone https://github.com/yourusername/Multimodal-Map-Search.git
cd Multimodal-Map-Search
```

### 2. Download embeddings

Download the three `.pt` files from [Google Drive](https://drive.google.com/drive/folders/161PYWfSHI393Qh6RPJolPopAGvaMffMq?usp=sharing) and place them in the same directory as `search.ipynb`.

### 3. Install dependencies

Create a virtual environment (optional but recommended) and install required packages:

```bash
pip install torch torchvision transformers gradio pillow
```

### 4. Run the notebook

Open `search.ipynb` and:
- Run the **first two cells** to load dependencies and prepare the search environment.
- Run the **last cell** to launch the **Gradio UI**.

---

## 🧪 Example Use Cases

- Search for **ancient maps** of a specific city or region.
- Compare **visual similarities** between different historical maps.
- Use in **educational settings** to teach geography, cartography, and history.

---

## 📁 Project Structure (Optional)

```
Multimodal-Map-Search/
│
├── search.ipynb               # Main notebook with search logic and UI
├── mapimg.pt                  # Embedding file (downloaded)
├── mapimg_idx.pt              # Index file (downloaded)
├── mapimg_normalized.pt       # Normalized embeddings (downloaded)
├── README.md                  # Project overview
└── requirements.txt           # (Optional) Dependencies list
```

---
##  Acknowledgments

- Based on OpenAI's [CLIP model](https://openai.com/blog/clip).
- Thanks to the creators of the dataset and embedding files.
- **For image-input search, the image input is not restricted to images from the Library of Congress.**

---
