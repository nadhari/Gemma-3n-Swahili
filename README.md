# Gemma-3n-Swahili: On-Device Universal Swahili AI Assistant

<div align="center">

[![Hugging Face](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Models-yellow)](https://huggingface.co/collections/Nadhari/gemma-3n-swahili-6893b845118de47136343522)
[![Demo](https://img.shields.io/badge/🚀-Live%20Demo-blue)](https://huggingface.co/spaces/Nadhari/Gemma-3n-Swahili-demo)
[![License](https://img.shields.io/badge/License-Apache%202.0-green.svg)](LICENSE)

</div>

## 🚀 Try It Now - No Installation Required!

**[→ Live Demo on Hugging Face Spaces](https://huggingface.co/spaces/Nadhari/Gemma-3n-Swahili-demo)**

Experience Gemma-3n-Swahili instantly in your browser - no downloads, no setup, just click and chat in Swahili!

## 📱 Run on Your Phone

Watch it in action: [📹 Phone Demo Video](https://youtube.com/shorts/K79-rfhQa-M?feature=share)

### iOS & Android Instructions:

1. **Download PocketPal AI**
   - [📱 iOS App Store](https://apps.apple.com/us/app/pocketpal-ai/id6502579498)
   - [🤖 Google Play Store](https://play.google.com/store/apps/details?id=com.pocketpalai)

2. **Search for the model** in the app:
   ```
   Nadhari/gemma-3n-swahili-E2B-it-gguf
   ```

3. **Download and start chatting** - It's that simple!

## 💻 Run on Desktop

### Quick Start with Ollama

```bash
ollama run hf.co/Nadhari/gemma-3n-swahili-E2B-it-gguf:Q8_0
```

### Enhanced Experience with Ollamate

For a better chat interface, use [Ollamate](https://github.com/humangems/ollamate) - check their repository for detailed installation instructions.

---

## 🌍 About Gemma-3n-Swahili

### The Challenge

Despite being spoken by over 200 million people across Sub-Saharan Africa, current AI models have limited Swahili comprehension and instruction following, leading to:

- Inability to maintain cultural understanding
- Limited support for code-switching common in modern Swahili usage
- Lack of specialized vocabulary for emerging technological concepts

### Introducing Gemma-3n-Swahili

Gemma-3n-Swahili represents a paradigm shift in how we approach low-resource language modeling. We've created models that excel specifically in Swahili while maintaining the ability to bridge to other languages when needed.

## 🤗 Model Collection

Explore our complete model collection on Hugging Face:

**[→ Gemma-3n-Swahili Collection](https://huggingface.co/collections/Nadhari/gemma-3n-swahili-6893b845118de47136343522)**

### Available Models

- **[gemma-3n-swahili-E2B-it](https://huggingface.co/Nadhari/gemma-3n-swahili-E2B-it)**: Balanced performance for resource-constrained environments
- **[gemma-3n-swahili-E4B-it](https://huggingface.co/Nadhari/gemma-3n-swahili-E4B-it)**: Optimal for general Swahili applications
- **GGUF Versions**: Quantized models for mobile and edge deployment

## 📊 Performance Benchmarks

Our models achieve significant improvements over base Gemma 3n on Swahili benchmarks:

### Swahili MMLU Results

Benchmarking results/swahili-mmlu/plots/overall_performance.png

### Translation Performance (Perplexity - Lower is Better)

[Benchmarking results/english-swahili-translation-bench/plots/translation_performance_comparison.png](https://github.com/nadhari/Gemma-3n-Swahili/blob/main/Benchmarking%20results/english-swahili-translation-bench/plots/translation_performance_comparison.png)

Benchmarking results/english-swahili-translation-bench/plots/translation_perplexity_comparison.png

These results demonstrate transformative gains in cross-lingual understanding.

## 🛠️ Technical Details

### Training Approach

We fine-tuned Gemma-3n models using:
- **Dataset**: 10,000 high-quality Swahili instruction-response pairs from Bactrian-X
- **Method**: LoRA fine-tuning with Unsloth framework
- **Focus**: Language-specific improvements while preserving multimodal capabilities

### Key Features
- ✅ Excellent Swahili understanding and generation
- ✅ Technical and creative writing capabilities
- ✅ Cultural context awareness
- ✅ Code-switching support
- ✅ On-device deployment ready


## 🚀 Quick Start for Developers

### Using Transformers

```python
from transformers import AutoModelForCausalLM, AutoTokenizer

model = AutoModelForCausalLM.from_pretrained("Nadhari/gemma-3n-swahili-E2B-it")
tokenizer = AutoTokenizer.from_pretrained("Nadhari/gemma-3n-swahili-E2B-it")

# Example usage
prompt = "Eleza kwa nini anga ni bluu?"
inputs = tokenizer(prompt, return_tensors="pt")
outputs = model.generate(**inputs, max_length=200)
response = tokenizer.decode(outputs[0], skip_special_tokens=True)
print(response)
```


## 🤝 Contributing

We welcome contributions! 

## 📄 License

This project is licensed under the Apache 2.0 License - see the [LICENSE](LICENSE) file for details.

##  Acknowledgments

- The Bactrian-X team for the Swahili dataset

## 📬 Contact

For questions, suggestions, or collaborations:
- Open an issue on GitHub
- Reach out on [Hugging Face](https://huggingface.co/Nadhari)

---

<div align="center">
Made with ❤️ f
</div>
