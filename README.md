# gen_ai_with_llm_coursera


## Syllabus:

1. Week 1: 
    * Introduction to LLMs and the generative AI project lifecycle:
        1. Prompt
        2. LLM
        3. Context Window.
        4. Complettion
        5. Inference
        6. Issues with Tradtional Text Generation (with LSTMs).
        7. Transformers
        8. Tokenizers
        9. Embedding Layers, Positional Embedding.
        10. Generating text with Transformers.
        11. Encoder Decoder models (BART, T5, etc.), Encoder only models (BERT, etc.), Decoder only models (GPT, LLAMA).
        12. Prompting, Prompt Engineering (In context learning, zero-shot inference, 1-shot inference, few shot inference).
        13. Generative Configuration (Max new tokens, Temperature, Greedy/Random sampling, Top-P, Top-K sampling).
        14. Gen AI Project Life Cycle.

    * LLM pre-training and scaling laws:
        1. Encoder only models, use cases, examples.
        2. Decoder only models, use cases, examples.
        3. Encoder Decoder models, use cases, examples.
        4. Computational challenges of training LLMs.
        5. Scaling laws and compute optimal models (Chinchilla).
        6. Pre-training for domain adaptation.
    
    * Quiz covering above topics.
    * Programming assignment on SageMaker:
        1. Set up Kernel and Required Dependencies.
        2. Summarize Dialogue without Prompt Engineering.
        3. Summarize Dialogue with an Instruction Prompt.
            1. Zero Shot Inference with an Instruction Prompt.
            2. Zero Shot Inference with the Prompt Template from FLAN-T5.
        4. Summarize Dialogue with One Shot and Few Shot Inference.
            1. One Shot Inference.
            2. Few Shot Inference.
        5. Generative Configuration Parameters for Inference.

2. Week 2: 
    * Instruction fine tuning (IFT)
        1. Catastrophic forgetting (and issues with in context learning, context window size, etc.)
        2. Single task instruction fine tuning.
        3. Multi task instruction fine tuning.
        4. Supervised fine tuning 
        5. Scaling instruct models (Quantization, 16 bit, 8 bit, 4 bit)
        6. Evaluating the task (using ROUGE and BLEU metrics).
        7. Evaluation of the LLM (using benchmarks).
    * PEFT and related techniques
        1. Issues with full fine tuning.
        2. Advantage of PEFT based fine tuning.
        3. Selective (training subset of parameters of LLM) PEFT.
        4. Reparaterization based PEFT (LORA: adding LORA matrices, fine tuning on these parameters).
        5. Additive PEFT (Soft Prompting, adding virtual tokens to inputs + fine tuning).
        6. Full fine tuning vs LORA performance (ROUGE metrics).
        7. Full fine tuning vs Soft Prompting (ROUGE metrics).
    
    * Quiz covering above topics
    
    * Programming assignment on SageMaker:
        1. Set up Kernel, Load Required Dependencies, Dataset and LLM
            1. Set up Kernel and Required Dependencies.
            2. Load Dataset and LLM.
            3. Test the Model with Zero Shot Inferencing.
        2. Perform Full Fine-Tuning
            1. Preprocess the Dialog-Summary Dataset.
            2. Fine-Tune the Model with the Preprocessed Dataset.
            3. Evaluate the Model Qualitatively (Human Evaluation).
            4. Evaluate the Model Quantitatively (with ROUGE Metric)
        3. Perform Parameter Efficient Fine-Tuning (PEFT)
            1. Setup the PEFT/LoRA model for Fine-Tuning.
            2. Train PEFT Adapter.
            3. Evaluate the Model Qualitatively (Human Evaluation).
            4. Evaluate the Model Quantitatively (with ROUGE Metric).
