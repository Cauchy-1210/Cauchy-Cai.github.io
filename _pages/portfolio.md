---
layout: archive
title: ""
permalink: /portfolio/
author_profile: true
---
# RFID Technology-Based Textile Production Process Defective Tracking and Quality Management System  
**Supervisor:** Prof. Zhengguo Sheng  

- **Objective:**  
  Establish an efficient and accurate yarn information tracing system using RFID and IoT technologies.  
- **Key Contributions:**  
  - Solved inefficiencies, incomplete data, and manual intervention in traditional yarn tracing methods.  
  - Enabled closed-loop information management from production → quality inspection → maintenance.  
  - Enhanced intelligence in textile production processes.  

---
# Meeting Transcription and Analysis System  

## Project Overview  
This project focuses on speaker recognition and voice separation tasks, targeting meeting minutes scenarios. It proposes an optimization scheme based on advanced deep learning models. Through system-level architecture design and fine-grained scheduling of computing resources, it ensures high recognition accuracy while significantly improving the execution efficiency and stability of multi-task concurrency.  

The system integrates the generated document content into a large language model for:  
- Automatic meeting summarization  
- Personal summary generation  
- Task assignment tracking  

## Core Innovations & Technical Contributions  

### Modular Model Architecture  
Adopts a heterogeneous model combination strategy, integrating four core modules:  

1. **Speech Recognition (Paraformer-large)**  
   - Non-autoregressive end-to-end architecture  
   - Supports 16kHz Chinese/English non-streaming recognition  

2. **Speech Activity Detection (FSMN-VAD)**  
   - Detects effective speech segments' start/end points  
   - Reduces recognition errors from invalid audio  
   - Adjustable segmentation granularity parameters  

3. **Punctuation Restoration (CT-Transformer)**  
   - Controllable delay Transformer architecture  
   - Maintains performance without distant future context dependency  

4. **Speaker Recognition (CAM++)**  
   - Frontend: Residual convolutional network  
   - Backbone: Time-delay neural network  
   - Context-aware Mask modules for noise suppression  

## System Optimization  

### Concurrency Handling  
- Implemented thread pool limitation  
- Fixed CPU over-utilization bugs  
- **Performance**: 1.5 minutes processing per meeting hour  

### Audio Enhancement  
- Mossformer2-based pre-denoising  
- Addresses real-world reverberation challenges  
- **Performance**: 2.5 minutes denoising per meeting hour  

