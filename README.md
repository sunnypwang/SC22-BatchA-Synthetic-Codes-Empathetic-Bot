# jAIce : The Empathetic Robot

## Empathetic Dialogue Generator 

###### _A project by Synthetic Codes_

### How to Use

cd into the `/app` folder...

Inside `main.py` file, edit the URL  to match the server your are running/

Then, run `python3 main.py` to start the server.

Next, open the link in the terminal to access the website.

Finally, locate the model section in our website to use jAIce.

### Technical Stack

- The datasets containing the prompts and empathetic responses (EmpatheticDialogues) https://github.com/facebookresearch/EmpatheticDialogues
- Python, pandas, and excel to preprocess the data.
- Python and aitextgen for the backend of the product demo
- GPT-2, the model to train on
- Google Colab servers to train the model
- HTML, CSS, and JavaScript to create the front end of the product demo
- Flask to connect the front end and the back end
- AI Camp servers to host the project on a domain

### Dataset

We used a novel dataset of ~25,000 conversations grounded in [Emotional situations](https://github.com/facebookresearch/EmpatheticDialogues).
We trained our model to imitate responses in the dataset.
To make sure only replies and not questions were generated, we removed all lines with questions as a response.
We also concatenated the speaker’s sentences for each response in a conversation so the model has the full situation for each response.

### Type of Model

We used the 124M (small) version of [GPT-2](https://openai.com/blog/better-language-models/), an open-source transformer model developed by OpenAI.
It is especially useful for text generation, hence why we were able to utilize it.
We fine-tuned the pre-trained model using the Empathetic Response dataset.
We used 10,000 steps to train the model.

We used [aitextgen](https://docs.aitextgen.io/) to train the model on Google Colab servers. Each model took ~30 minutes to train, which is 6 minutes/1000 steps.

### Libraries Used

We used <u>pandas</u> to preprocess the data.  
To train the model, we used <u>aitextgen</u>.  
To connect the frontend to the backend, we used <u>flask</u>.

### About the Team

We are a group of awesome people at AI camp to make cool natural language processing products.

Team Members:

- **Chandrark Muddana**  
  Product Manager  

- **Chris Sanrow**  
  Lead Back End Developer  

- **Jayce Chanas**  
  Lead Front End Developer  

- **Victoria You**  
  Front End Developer  

- **Riya Kumar**  
  Back End Developer  

- **Phakawat Wangkriangkri**  
  Mentor  

