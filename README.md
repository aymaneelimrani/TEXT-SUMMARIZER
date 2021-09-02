## Implementation of 'Pretraining-Based Natural Language Generation for Text Summarization'



### Preparing package/dataset
0. Run: `pip install -r requirements.txt` to install required packages
1. Download chunk CNN/DailyMail data from: https://github.com/JafferWilson/Process-Data-of-CNN-DailyMail
2. Run: `python news_data_reader.py` to create pickle file that will be used in my data-loader

### Running the model
For me, the model was too big for my GPU, so I used smaller parameters as following for debugging purpose. 
`CUDA_VISIBLE_DEVICES=3 python main.py --cuda --batch_size=2 --hop 4 --hidden_dim 100`
