# A PyTorch implementation of the groundbreaking ResNet architecture that revolutionized deep learning

What is the problem with convergence? With the network depth increasing, accuracy gets saturated and then degrades rapidly." - He et al., 2015
This repository contains a clean, well-documented implementation of Residual Networks (ResNet) from the seminal paper by Kaiming He, Xiangyu Zhang, Shaoqing Ren, and Jian Sun that won the 2015 ImageNet Challenge.
✨ What Makes This Special?

🏗️ Clean Architecture: Modular design with residual blocks
📊 Multiple Variants: ResNet-18, 34, 50, 101, 152 implementations
⚡ Optimized Training: Skip connections that solve vanishing gradients
🎯 SOTA Results: Achieves paper-level accuracy on ImageNet
📝 Well Documented: Every component explained with comments

🧠 The Big Idea
Traditional deep networks suffer from the vanishing gradient problem - the deeper you go, the harder it becomes to train. ResNet introduced skip connections (residual connections) that allow gradients to flow directly through the network:
Traditional: x → conv → relu → conv → relu → output
ResNet:     x → conv → relu → conv → (+) → relu → output
            └─────────────────────────┘
                  (skip connection)
This simple yet powerful idea enabled training of networks with 152+ layers while maintaining (and often improving) accuracy!
🏛️ Architecture Overview
| Model | Layers | Parameters | ImageNet Top-1 | ImageNet Top-5 |
|-------|--------|------------|----------------|----------------|
| ResNet-18 | 18 | 11.7M | 69.76% | 89.08% |
| ResNet-34 | 34 | 21.8M | 73.31% | 91.42% |
| ResNet-50 | 50 | 25.6M | 76.15% | 92.87% |
| ResNet-101 | 101 | 44.5M | 77.37% | 93.56% |
| ResNet-152 | 152 | 60.2M | 78.31% | 94.06% |
