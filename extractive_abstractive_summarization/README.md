# Training  model
# require train,test,valid,embedding pickle in current directory to run also needed revise train,valid,test data
# it will print the loss and rouge_score every epoch both for train data and valid data
# it will save state_dict if rouge-1 score for current epoch is better than all previous rouge-1 score
# it will write a file call loss_train_adl_64_LSTMHID_1.txt to store the training result
python3.7 seq_tag_train.py
python3.7 seq2seq_train.py


# plot relative location
# require valid.pkl and valid.json to plot the result
# it wiil calculate,print rouge-score and plt the relative location plot on the valid data
python3.7 seq_tag_val.py

#plot attention plot
#using the function in drawattn.py to plot attn plot



