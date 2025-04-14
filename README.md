# TP3-Team-3
  Large language models, commonly known as LLMs, are a form of Artificial Intelligence that are used to generate and respond to text. Large Language Models were first developed under the initiative of ChatBot usage, but have since expanded far beyond that. In the early 2020’s there was a surge of widespread LLM recognition as highly capable models such as GPT were introduced to the public. While LLMs may be beneficial for personal enjoyment, this project asserts the idea the LLMs have value within professional contexts as well. 
  
  The methodology used to create LLMs stems from Recurrent Neural Networks. Recurrent Neural Networks are a type of deep learning model that processes data sequentially. Unfortunately, Recurrent Neural Networks tend to put too large of an emphasis on the most recent words, and struggle to incorporate longer term memory. Large Language Models similarly focus on encoding and decoding text, but incorporate two key elements: attention and transformers. Instead of just focusing on the most recent words, attention allows the model to calculate the contextual importance of all other previous words in order to predict the next word more accurately. The transformer aspect removes the need for sequential processing altogether by allowing the model to process all words in a sentence simultaneously. Transformers and attention contribute to Large Language Models ability to quickly generate coherent, situationally valid text that relies on the entirety of the passage. 
  
  Large Language Models can be beneficial for both internal and external use. When communicating with customers, LLMs and chatbots can be essential for quickly responding to questions, troubleshooting problems, and even making product recommendations based on desired needs. Additionally, LLMs can be an asset for employees too. They can draft and summarize documents, streamline access to pertinent information, and even help guide decisions. One specific application of LLMs presented at the 2024 AAAI Conference on Artificial Intelligence describes “How Teachers Can Use Large Language Models and Bloom’s Taxonomy to Create Educational Quizzes” (Elkins 2024). The study included testing three different quiz generation techniques: handwritten, simple, and controlled. The first included handwriting questions, the second included generating quiz questions from GPT 3.5 using simple prompts, and the third included generating quiz questions from GPT 3.5 using example questions crafted by domain experts and Blooms Taxonomy framework. All three techniques focused on generating questions from Wikipedia literature passages. As a result of the study, it was found that there was no significant loss of quality with the LLM generated questions but there was an overwhelming preference for the controlled generation technique from teachers. In addition to reducing the time it takes to create quiz questions as presented in the article, LLMs can also assist teachers in lesson planning and students in understanding complex topics by breaking down difficult concepts, answering questions in real time, and offering personalized study support. LLMs have the potential to simultaneously enhance both teacher and student experiences. 
  
  Within the coding section of this project, we included two different models, and used vibe coding to create a website. The first model was a language model using TensorFlow to present a simplified version of how LLMs learn from and generate text. We trained the model using a fifth-grade science textbook. Each unique word was pulled from the text, encoded as a number, and stored in a dataset called a vocabulary. The model learned from the textbook sequentially, meaning it processed one word at a time in order, using the context of previous words to predict the next one. This structure is a type of Recurrent Neural Network called a Long Term Short Term Memory since it reincorporated weights from earlier parts of the text too. The second model implemented GPT-2, an open-source pretrained model developed by OpenAI that is accessible through Keras. Unlike our first model, the second language model uses both attention and transformers to build context into the predictions as highlighted earlier. This model also calls attention to the use of randomness within GPT models as the resulting word predictions often vary. For the vibe coding section, the system accepts a textbook in text file format and can return summaries, lesson plans, and suggested activities.
  
  When input with the same prompt, each of the two models resulted in very different outputs. While the first was able to form a few sentences, the minimal size of the training textbook resulted in a very limited vocabulary and a lack of a coherent output. The model that incorporates GPT-2 on the other hand, was able to successfully finish the prompt with an understandable output. The discrepancy between these two model outputs presents one of the biggest challenges in the creation of LLMs: computational complexity. High-performing models like GPT-2 require extensive datasets, significant computing power, and long training times to achieve their level of fluency and contextual awareness. This complexity makes developing large-scale models from scratch inaccessible to most organizations. While building off existing LLMs may pose as an option, the most advanced models often have fees. Furthermore additional boundaries preventing many firms from using existing LLMs includes both data privacy and erroneous responses.
  
  In the case of academic LLM applications, many private student and teacher models such as Khanmigo, Eduaide.ai, and MagicSchool.ai have been created. While these models do have fees acompanying them, they are more suited to education in comparison to open source models. However, it’s important to recognize that even the most advanced models can produce errors. Unfortunately, inaccurate responses can be detrimental to students who learn to trust outputs. Similarly, bias in training data can also lead to reinforcement or teaching of stereotypes. Despite these limitations, the potential for LLMs to become a key asset within education is anticipated. As technology continues to advance, it is likely the capabilities and accessibility of LLMs will too. This will allow for the use of LLMs across a wide range of industries to continue expanding.

Creators: 
[Fiona Basewitz](https://github.com/fcbasewitz/Profile/blob/main/README.md)
[Rachael Lee](https://github.com/relee713/hello_world?tab=readme-ov-file#hobbies)
[Ben Greenberg](https://github.com/BenGreenberg31)
[Mattijs Lasore](https://github.com/mlasore26/profile)

Sources:

Elkins, S., Kochmar, E., Cheung, J. C. K., & Serban, I. (2024). How Teachers Can Use Large Language Models and Bloom’s Taxonomy to Create Educational Quizzes. Proceedings of the AAAI Conference on Artificial Intelligence, 38(21), 23084-23091. https://doi.org/10.1609/aaai.v38i21.30353
TensorFlow Authors. (n.d.). Text generation with an RNN. TensorFlow. https://www.tensorflow.org/text/tutorials/text_generation
Qian, C. (2023, April 17). GPT-2 text generation with KerasNLP and Keras Hub. Keras. https://keras.io/examples/generative/gpt2_text_generation_with_keras_hub/
