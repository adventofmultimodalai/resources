## Welcome to the Multimodal Gen AI Hack, hosted by Intel Liftoff! 🚀

This hackathon focuses on Multimodal Generative AI, which enables you to create applications that combine various data types, such as text, images, and audio. You can explore two main approaches:

🔧 The Engineering-Driven Approach: Combine specialized models for each modality to create a tailored pipeline. For instance, you could use Whisper for audio transcription, pass the text to an LLM like Llama 3.1 for generating creative prompts, and then visualize the output using an image generation model like Stable Diffusion. This modular approach is well-suited for tasks such as developing an AI-driven content creation pipeline or an interactive storytelling system.

🌐 The Pure Multimodal Model Approach: Utilize state-of-the-art models like LLaVA-NeXT or Moondream, which integrate vision transformers (ViT) and LLMs into a single model. These models can process multimodal inputs end-to-end, enabling applications like visual question answering, where the system can comprehend an image and respond to queries about its content. For example, you could create an AI agent for retail that analyzes product shelf images and takes action by generating insights about restocking, suggesting promotions, or notifying relevant teams.

To make things even more exciting, we have a variety of prizes up for grabs, thanks to our fantastic startup partners in the Liftoff program. 


## Dive into the World of Generative AI

Dive into the world of generative AI and keep the spirit of innovation alive. Check out the [challenges](https://github.com/adventofmultimodalai/challenges) and [resources](https://github.com/adventofmultimodalai/resources) to start your own GenAI journey today!

<div align="center">
  <img src="https://github.com/user-attachments/assets/a719fc12-337b-429b-affe-c9508200740b" alt="Generative AI" />
</div>

Hello, AI Adventurers! Ready to navigate the exciting world of Generative AI with us? Here's everything you need to ace the [Advent of MultiModal AI](https://adventaihacks.com) hackathon:

### Model APIs for the Hackathon

We’ve prepared API endpoints for text generation and image generation to power your hackathon projects. You can use these APIs to interact with models like LLaVA-Next, Phi3, and Flux.  

- 📄 **[API Documentation for hosted LLM and Image Generation Models](https://github.com/adventofmultimodalai/resources/blob/main/api.md)**: Learn how to access and use the APIs.
- 🚀 Start building innovative applications by leveraging these endpoints today!


### GenAI GitHub Repositories

1. **GenAI Playground on Intel GPUs**  
   [GitHub Repository](https://github.com/rahulunair/genAI)  
   A set of iPython notebooks from Stable Diffusion to LLMs.

2. **Intel AI Use Cases for GenAI**  
   [GitHub Repository](https://github.com/rskasturi/usecases)  
   Key insights on GenAI applications, including Stable Diffusion, LLM inference, fine-tuning, and code generation with Intel GPUs.  

3. **Diffusion Model Serving with Ray on Intel Data Center Max Series GPUs**  
   [GitHub Repository](https://github.com/rahulunair/xpu_ray)  

4. **Gen AI model Deployments on Intel Data Center Max Series GPUs**  
   [Tiber AI community](https://tiberaicommunity.github.io)  
   A collection of deployment docs for LLM and image models.

5. **LLaVA-NeXT Multimodal Chatbot with OpenVINO**  
   [Notebook Link](https://docs.openvino.ai/2024/notebooks/llava-next-multimodal-chatbot-with-output.html)  
   A practical example of building optimized multimodal chatbots combining vision and language with OpenVINO.


---

### Intel Developer Cloud
   
- 🌐 Step into the [Intel Tiber AI Cloud](https://cloud.intel.com) (IDC), register for free, and access Intel Xeon CPUs, GPUs, & HPUs. Discover a set of curated notebooks for Stable Diffusion, LLM inference, fine-tuning, and more under the `Learning` section.
- **This will give you access to:** 
  - **Jupyter Notebook:** Work within a Jupyter Notebook environment, optimized for Generative AI challenges.
  - **Disk Space:** Up to 30GB per user (depending on availability).
  - **GPU:** Intel GPU with 48GB memory (Data Center Max 1100), tailored for AI applications.
  - **HPU:** Intel Gaudi2 (Habana) with 96GB memory, ideal for Gen AI applications.

---

### How to Build and Deploy Your Application

We recommend starting with the **free Jupyter notebooks** available in the **Learning** section for experimentation. These notebooks are perfect for:

- Prototyping your project with AI models like Stable Diffusion and LLMs in a pre-configured environment.
- Experimenting with Generative AI workflows before deployment.

💡 **Need dedicated Hw for deployment?** While Jupyter notebooks are ideal for experimentation, they are not suited for production deployments. If your project requires **dedicated compute resources for deployment**, let us know. We may provide access to **Intel GPU or CPU VMs** on a **limited, case-by-case basis** due to resource constraints.

---

### Building Outside the Cloud

If you're using only the hosted APIs we’ve provided, feel free to build your project on any platform of your choice. However:

- **⚠️ Important:** Using other hosted API services for this challenge is not allowed.  
  This ensures fair usage and encourages participants to explore the tools and resources we’ve specifically made available.

---

Start your journey with the Intel Tiber AI Cloud today and unleash your creativity in Generative AI! 🚀


---

### Intel Geti and Resources:
- **Access to Intel Geti:** [https://intel.ly/3VoxZ7V](https://intel.ly/3VoxZ7V)
- **Intel Geti:** [https://app.geti.intel.com/](https://app.geti.intel.com/)
- **Documentation:** [https://docs.geti.intel.com/cloud/guide/get-started/introduction.html](https://docs.geti.intel.com/cloud/guide/get-started/introduction.html)
- **Geti SDK:** [https://github.com/openvinotoolkit/geti-sdk](https://github.com/openvinotoolkit/geti-sdk)
- **OpenVINO Test Drive:** [https://github.com/openvinotoolkit/openvino_testdrive](https://github.com/openvinotoolkit/openvino_testdrive)


<a name="prediction-guard"></a>
### Prediction Guard: Access a variety of privacy-conserving LLMs, validate outputs
   - 🛡️ Explore [Prediction Guard Documentation](https://docs.predictionguard.com). Check out the "Getting Started" and "Using LLMs" pages to run your first text or chat completions with the Prediction Guard API or Python client.

      ```python
      import os
      import json
      import predictionguard as pg
   
      os.environ['PREDICTIONGUARD_TOKEN'] = "<your PG access token>"
   
      response = pg.Completion.create(
         model="Neural-Chat-7B",
         prompt="The advent of Gen AI hackathon is: "
      )
   
      print(json.dumps(
         response,
         sort_keys=True,
         indent=4,
         separators=(',', ': ')
      ))
      ```

   - 💪 Run through some of the examples in the [Using LLMs](https://docs.predictionguard.com/usingllms/accessing) section of the docs to learn more about basical prompting, prompt engineering, retrieval, chat, agents, etc.
   - 🌐 Dive into the [Multimodal Capabilities](https://docs.predictionguard.com/options/lvms) supported by Prediction Guard APIs to build intelligent, multi-modal AI solutions.


---

### Intel XPUs (GPUs) and Intel Extension for PyTorch ( required to use XPUs):**
   - 🔥 Check if XPU is ready:
     ```python
     import torch
     import intel_extension_for_pytorch
     print(f"torch.xpu.is_available()")
     ```
   - 📚 Dive deeper at [Intel XPU Tutorials](https://intel.github.io/intel-extension-for-pytorch/xpu/latest/tutorials/examples.html)

---

**Detect Your AI Resources: The Discovery Commands**
   - 🔍 Uncover Intel GPUs and CPUs:
     ```bash
     echo "Intel GPUs:"
     xpu-smi  discovery 2> /dev/null
     echo "Intel Xeon CPU:"
     lscpu | grep "Model name"
     xpu-smi dump -m 18
     ```
---

### Python Package Installation: Effortlessly
   - 📦 Streamline your installations:
     ```python
     import sys
     import site
     from pathlib import Path
     !echo "Installing..."
     !{sys.executable} -m pip cache purge > /dev/null
     !{sys.executable} -m pip install <python_package_name>
     !echo "Installation Complete."
      def get_python_version():
          return "python" + ".".join(map(str, sys.version_info[:2]))
      
      def set_local_bin_path():
          local_bin = str(Path.home() / ".local" / "bin") 
          local_site_packages = str(
              Path.home() / ".local" / "lib" / get_python_version() / "site-packages"
          )
          sys.path.append(local_bin)
          sys.path.insert(0, site.getusersitepackages())
          sys.path.insert(0, sys.path.pop(sys.path.index(local_site_packages)))
      
      set_local_bin_path()
     ```
   
**Craft Your Custom Conda Environment**
   - 🧪 Mix your perfect environment:
     ```bash
     conda clone pytorch-gpu <new_name>
     conda activate new_name
     conda install ipykernel
     ipykernel install <>
     conda install ...
     ```
     
### Vector Databases: Exploring with LanceDB
    - 🗂️ Engage with [LanceDB VectorDB Recipes](https://github.com/lancedb/vectordb-recipes/tree/main/examples/multimodal_clip_diffusiondb)

**Mastery in Retrieval Augmented Generation and Multi Modals**
   - 🎓 Learn from [LangChain]([https://python.langchain.com/docs/use_cases/question_answering/](https://python.langchain.com/docs/how_to/#multimodal)) and [Llama-index](https://docs.llamaindex.ai/en/stable/use_cases/multimodal/)


### AgenticFlow AI by Pixel ML
Build and deploy your solutions using [AgenticFlow AI](https://agenticflow.ai/), a powerful platform for creating AI-powered marketing workflows. Get started with:
- 📚 [Documentation](https://docs.agenticflow.ai/)
- 🛠️ [Pre-built workflow templates](https://agenticflow.ai/app/explore)
- 🤖 No-code AI automation tools


### Additional Resources

- **[A Comprehensive Guide to Multimodal LLMs and How They Work](https://www.ionio.ai/blog/a-comprehensive-guide-to-multimodal-llms-and-how-they-work)**  
  This blog explores how to integrate different modalities using specialized models, providing a clear roadmap to build versatile multimodal applications.

- **[Guide to Building Multimodal RAG Systems](https://www.analyticsvidhya.com/blog/2024/09/guide-to-building-multimodal-rag-systems/)**  
  A detailed guide on constructing retrieval-augmented generation (RAG) systems combining text, images, and other data formats to handle diverse use cases.

## Challenge tutorials
### Challenge 1: AI Meme Factory
**Skill Level: Great for Getting Started**

Build a workflow that generates memes by analyzing user-inputted text or emotions. The system should:
- Detect sentiment from user input
- Select or generate appropriate meme templates
- Overlay text captions
- Produce memes that resonate with the intended emotion or message

<div align="center">
  <img src="https://photoshot-us.s3.us-east-1.amazonaws.com/next-s3-uploads/5d1861b8-2958-42eb-93a2-77b513499a42/Challenge-1.png" alt="AI Meme Factory Challenge" />
</div>

📺 [Watch Tutorial Video](https://qra.ai/intelmeme)

### Challenge 2: Multi-Modal Story Generator
**Skill Level: Moderate Challenge**

Create an application that transforms user prompts or product specifications into engaging stories or marketing narratives. Your solution should:
- Generate comprehensive content for storytelling or product promotion
- Create illustrative images to accompany the narrative
- Combine multiple modalities for engaging content creation

<div align="center">
  <img src="https://photoshot-us.s3.us-east-1.amazonaws.com/next-s3-uploads/1fe28e32-584b-456d-ae6c-f795bf8e4e8a/Challenge-2.png" alt="Multi-Modal Story Generator Challenge" />
</div>

📚 [View Tutorial](https://qra.ai/intelcontent)


## Contributing 🤝

**Share Your Genius:**
- Fork the repository, push your changes, and open a pull request.
- Remember, every bit of contribution helps us sail further in the ocean of AI!

## Reporting Issues 🐛

**Spot Something Amiss?**
- Stumbled upon a typo or facing a challenge? Let us help! 🛠️
- Create an issue in the [GitHub repository](https://github.com/adventofmultimodal/resources/issues) with a detailed description.

