# place the dataset .csv file in dataset dir

# choose the target feature, Here the target feature is Sales

1. Create environmnet and activate it.   #use this command - python -m venv atfnet_env
2. install requirement from requirement.txt file. #using this command - pip install -r requirements.txt
3. to train the model Run " py run.py --data_path retail_sales.csv --model_id ETTh1_96_96 --model ATFNet --data custom --features H --seq_len 96 --label_len 24 --pred_len 96 --e_layers 2 --d_layers 1 --enc_in 7 --dec_in 7 --c_out 7 --freq h --des Exp --itr 1 --train_epochs 100 --batch_size 256 "

    --data_path : dataset path
    --model_id  : model id present in the script file "./scripts/sales_rate/ATFNet.sh"
    --model     : name of the model
    --data      : custom dataset which shoul be modified according to the dataset
    --features  : targeted "Sales" feature which is mentioned as S in custom_dataset function
    --freq      : here "h" is mentioned which is hourly based prediction# Sales_prediction_ATFNet
