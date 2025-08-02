# 🍽️ AI-Chef: Intelligent Food Analyzer

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.28%2B-red)](https://streamlit.io/)
[![AI Models](https://img.shields.io/badge/AI-Gemini%20%7C%20Qwen-yellow)](https://github.com/Jebin-05/AI-Chef)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

An intelligent AI-powered food analysis application that uses advanced vision-language models to provide comprehensive culinary insights. Simply upload a food image and get detailed analysis including ingredients, recipes, nutrition facts, and cooking instructions.

## ✨ Features

### 🔍 **Smart Food Analysis**
- **Ingredient Detection**: Identify ingredients, spices, and seasonings with quantities
- **Recipe Generation**: Step-by-step cooking instructions from prep to serving
- **Nutrition Analysis**: Detailed calorie breakdown and macronutrient information
- **Food Validation**: Automatically verifies if uploaded images contain food items

### 🤖 **Multiple AI Models**
- **Gemini AI**: Fast cloud-based analysis (requires API key)
- **Qwen2-VL-7B**: Advanced local model with high accuracy
- **Custom prompts**: Specialized prompts for different analysis types

### 📱 **User-Friendly Interface**
- Clean Streamlit interface
- Multiple analysis modes (ingredients, recipe, nutrition, custom questions)
- Support for JPG, PNG, and WEBP image formats

## 🚀 Quick Start

### 1. Clone the Repository
```bash
git clone https://github.com/Jebin-05/AI-Chef.git
cd AI-Chef
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Configure API Keys (Optional - for Gemini)

Create a `.env` file in the project root:
```bash
GEMINI_API_KEY=your_actual_api_key_here
```

**Get Gemini API Key:** Visit [Google AI Studio](https://makersuite.google.com/app/apikey)

### 4. Run the Application

Choose from the available interfaces:

#### Main Application (Recommended)
```bash
streamlit run app.py
```

#### Gemini AI Interface (Cloud-based)
```bash
streamlit run gemini.py
```

The app will open in your browser at `http://localhost:8501`

## 📱 How to Use

### 🎯 **Simple 4-Step Process**

1. **📷 Upload Image**: Click the upload area and select a food image
2. **🔍 Choose Analysis**: Select from four analysis types:
   - 🥕 **Get Ingredients**: Complete ingredient list with quantities
   - 👨‍🍳 **Get Recipe**: Step-by-step cooking instructions  
   - 🔥 **Get Calories**: Detailed nutrition and calorie analysis
   - 💬 **Ask Questions**: Custom queries about the food
3. **🤖 AI Analysis**: Advanced AI models process your image
4. **📊 Get Results**: Receive detailed, professional analysis

### 💡 **Example Questions**
- "How do I make this dish step by step?"
- "What are the main ingredients and their quantities?"
- "How many calories are in this meal?"
- "What cuisine is this from?"
- "Is this dish healthy for my diet?"
- "What cooking techniques are used here?"

## 🏗️ Project Structure

```
AI-Chef/
├── app.py                  # Main Streamlit application
├── gemini.py              # Gemini AI interface
├── prompts.py             # AI prompts for different analysis types
├── requirements.txt       # Python dependencies
├── README.md             # Project documentation
└── .env                  # Environment variables (create this)
```

## 🤖 AI Models

### **Model Comparison**

| Model | Processing | Speed | Accuracy | Hardware Req. | Internet |
|-------|------------|-------|----------|---------------|----------|
| **Gemini 1.5 Flash** | Cloud | ⚡ Fast | 🎯 High | 💻 Low | ✅ Required |
| **Qwen2-VL-7B** | Local | 🐌 Medium | 🎯 Very High | 🖥️ High | ❌ No |

### **Specialized Prompts**
- **Ingredients Analysis**: Professional culinary analyst prompts
- **Recipe Generation**: Master chef-level cooking instructions
- **Nutrition Analysis**: Certified nutritionist approach
- **Food Validation**: Strict food detection algorithms

## 🔧 Requirements

### **Hardware Requirements**
- **Minimum**: 4GB RAM, 2GB free storage
- **Recommended for Qwen**: 16GB RAM, CUDA-compatible GPU
- **Internet**: Required only for Gemini model

### **Software Requirements**
- Python 3.8 or higher
- Modern web browser
- CUDA drivers (optional, for GPU acceleration)

## 🛠️ Installation Tips

### **For GPU Support (Optional)**
```bash
# Install PyTorch with CUDA support
pip install torch torchvision --index-url https://download.pytorch.org/whl/cu118
```

### **Common Issues**
- **Large model downloads**: Qwen model (~15GB) downloads automatically on first use
- **Memory issues**: Use Gemini API if you have limited RAM
- **API errors**: Ensure your Gemini API key is correctly set in `.env`

## 🤝 Contributing

We welcome contributions! Here's how you can help:

1. **Fork** the repository
2. **Create** a feature branch: `git checkout -b feature/amazing-feature`
3. **Commit** your changes: `git commit -m 'Add amazing feature'`
4. **Push** to the branch: `git push origin feature/amazing-feature`
5. **Open** a Pull Request

### **Areas for Contribution**
- 🐛 Bug fixes and improvements
- ✨ New AI models integration
- 🎨 UI/UX enhancements
- 📚 Documentation improvements
- 🧪 Test coverage expansion

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🆘 Troubleshooting

### **Common Solutions**

**API Key Issues:**
```bash
echo "GEMINI_API_KEY=your_key_here" > .env
```

**Dependencies:**
```bash
pip install --upgrade streamlit transformers torch
```

**Memory Issues:**
- Use Gemini API instead of local models
- Close other applications to free RAM
- Consider cloud deployment for heavy models

**Image Upload Issues:**
- Supported formats: JPG, PNG, WEBP
- Maximum recommended size: 10MB
- Ensure image clearly shows food items

## 🌟 Acknowledgments

### **Technologies Used**
- [Streamlit](https://streamlit.io/) - Web application framework
- [Google Gemini](https://deepmind.google/technologies/gemini/) - Advanced multimodal AI
- [Qwen-VL](https://github.com/QwenLM/Qwen-VL) - Open-source vision-language model
- [Hugging Face Transformers](https://huggingface.co/transformers/) - ML model library
- [PyTorch](https://pytorch.org/) - Deep learning framework

---

## 🚀 **Get Started Now!**

1. Clone the repository
2. Install dependencies
3. Run `streamlit run app.py`
4. Upload a food image
5. Discover the power of AI culinary analysis!

**Made with ❤️ for food enthusiasts and developers**

*Transform any food image into comprehensive culinary insights with AI!*
