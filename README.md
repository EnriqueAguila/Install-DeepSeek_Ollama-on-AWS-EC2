# Install-DeepSeek_Ollama-on-AWS-EC2
Instalar los modelos Ollama y DeepSeek en una instancia de EC2 de tipo G4 con Ubuntu.
![deepseek ec2](https://github.com/user-attachments/assets/d534252e-422a-413d-8dc2-acd1a9949512)
Installing DeepSeek on an AWS EC2 instance offers a number of significant benefits for accelerating language and machine learning models. With DeepSeek, you can Accelerate inference – DeepSeek leverages the GPU architecture of EC2 instances to accelerate language model inference, significantly reducing response times.
You can also improve efficiency – by using DeepSpeed ​​technology, DeepSeek optimizes instance resource usage, enabling higher performance with fewer resources.
Scalability – EC2 instances offer a wide range of scalability options, allowing you to fine-tune resources based on the needs of your model.
AWS integration – AWS integration allows for easy instance setup and management, as well as access to other AWS services for increased functionality.
Reduce costs By leveraging the efficiency of DeepSeek and the scalability of EC2 instances, you can significantly reduce the costs of running your
Installing DeepSeek on an AWS G4 EC2 instance can offer several benefits, especially if you are using artificial intelligence (AI) or machine learning (ML) models that require accelerated processing capabilities.

DeepSeek is a language model that combines machine learning techniques with logical reasoning to answer questions and perform reasoning tasks. Although DeepSeek is based on an LLM, it also incorporates logical reasoning components, making it a hybrid model that combines the strengths of both approaches.
In short, although DeepSeek is based on an LLM, it also incorporates logical reasoning components, making it a model that combines the strengths of both approaches. However, it is not a pure Reasoning Model, as its main focus remains on natural language processing.

Billion parameters

To run this model our computer must have as requirements, an Nvidia 3090 GPU graphics card
-64 GB of RAM
-an Intel i9 processor 10850k 10 cores and 20 logical processors
-and we must run it on UBUNTU 24.04 system

----------------------------------------------------------------------------------------------------------------------------------------------------------------

First install Ollama ollama.com

sudo ufw allow 11434/tcp

sudo apt update && sudo apt upgrade

sudo apt install curl

curl --version

In Ollama you click on download and copy the installation url
the one that says install with command

curl -fasthttp-----
paste and enter

in the ollama search engine you search for deepseek-r1
there are several models there but you choose the smallest 1.5 million parameters.
A parameter (also known as a weight or coefficient) is a numerical value used to adjust the output of a neuron or layer of the neural network.

1.5 million parameters" probably refers to the total number of weights, biases, and other parameters that are adjusted during training of a particular neural network.
To put this into perspective, 1.5 million parameters is a relatively large number, suggesting that the neural network is quite complex and may require a lot of training data and computational resources to train it properly.

1.5, weighs one gigabyte

you can put 32b
when you select it, it gives you a run, you copy it
and replace run with pull

ollama pull deepseek-r1:32b

since it's 20 gigabytes it can take a few minutes

pip list

ollama list

ollama run deepseek-r1:14b

I'm asked the question >>>

>>>how many inhabitants does Brazil have?
