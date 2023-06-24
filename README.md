# Title: Cryptocurrency Data Analysis and Vizaliation

Brief summary: <br>
This folder contains code and datasets download link for testing and analyzing New York city taxi trips. The specific technique considered describe the geographic range of the taxi trips, average computed trip distance, and vizualize the results in graphs, plots, and indicate on the New York city map.

Team: <br>
Afzal Hossain <br>
Department of Electrical and Computer Engineering <br>
Dr. Tyler Conlon <br>
Data Science Program <br>
Clarkson university <br>
Potsdam, New York 13699 <br>

Source Code Organization: <br>
    source_code.ipynb - This Python file has the necessary code for automatically testing the taxi trip data and vizualizez the results.

map_NYC.png/: Sample image of New York city

dataset_drive_link.txt/: This file contains the drive link of the required data.

version_requirements.txt/: Verrsion required to run the code.

Disclaimer:  <br>
There are no guarantees made about the accuracy or safety of this source code. This project was created for research purposes. The authors have attempted to produce code that is both accurate, efficient, and safe, but only limited testing has been performed. The authors of this code shall not be held accountable for any damage caused by using this code or any derivative works.

Platform and Installation: <br>
Python is needed to run the code. <br>
     a. Download Anaconda (https://docs.anaconda.com/anaconda/install/) or, Python 3.9.13 <br>
     b. Install the Python packages using the anaconda prompt according to the provided "version_requirements.txt" file.

Dataset:  <br>
The dataset contains two csv files where information are provided of taxi trips in New york city. The files are uploaded to drive and the link is is provided in the "dataset_drive_link.txt/" file.

Usage: <br>
     a. Download "source_code.ipynb" file and also download the data from the given drive link. <br>
     b. Run the python file with the csv data file within the same folder location.

Commands: <br>
source_code.py

CPU information: <br>
		Processor- Intel(R) Core(TM) i7-10700K CPU @ 3.80GHz  3.79GHz <br>
		RAM- 16.0 GB

# Analyzed results:  The followings provide information about the data and analyzed results from the dataset of Cryptocureencies


I have done a Cryptocurrency Data Analysis here. And using other dataset, which have effect on the cryptocurrency price, I have found the correlation between the 
Bitcoin Price and other factors like BTC price, BTC hash rate, BTC_difficulty etc. I have developped the code in google colab. Here, the following picture gives an overview of my code that how I have organised everthing in eight different steps.

![Capture](https://user-images.githubusercontent.com/83153124/207223979-32f94ce9-246d-423f-aa7f-321754aa049b.PNG)

## STEP 1: Importing all the necessary libraries
I have imported all the necessary libraries at the beginning which we need to import to run the code. For example, I have used the matplotlib and plotly libraies of python to plot and visualze the information properly.

## STEP 2: Importing the cryptocurrency dataset and analyzing it
Here, I have imported the cryptocurrency dataset where we have the information of stock prices of different cryptocurrencies.

![Capture2](https://user-images.githubusercontent.com/83153124/207225219-ab34dacd-6677-495c-a11d-3c0e5ad1b0a7.PNG)

In this dataset we have information of cryptocurrencies like Bitcoin, Ethereum, Dash etc. In the following image you can see the information (i.e, volumne) of different cryptocurrencies that we have in our dataset.

![Capture3](https://user-images.githubusercontent.com/83153124/207225589-c9280d49-672f-41a2-a07b-5e57a1f71894.PNG)

I have also got the mean, standar, min & max, and several other information of the dataset.

![Capture4](https://user-images.githubusercontent.com/83153124/207225950-ffdcded4-a105-43ff-8eb5-3eda5ebcf4bf.PNG)

## STEP 3: Data Visualization- All top Cruptcurrencies
In this step I have just done some visualization of our dataset in a catchty way.

![Capture5](https://user-images.githubusercontent.com/83153124/207226478-03bfecfe-72a8-4747-86c7-4230ff04d01f.PNG)

## STEP 4: Analyzing volume & price and comparison between currancies
I have plotted the volume and price information of the cryptocurrency dataset here to make it easily undesrstandable. And then I have done some plotting showing the comparisons between the cryptocurrencies.
Here, you can see the Pie Charts of our dataset which refers to the volmue of different cryptocurrencies through the year from 2015 to 2020/21. We can see that the Tether had the maximum volume (36.7%) in stock market which was larger than Bitcoin volume (34.7%) at that time. And we can also identify that some cryptocurrencies have only small portion of volume like 0.152%, 0.389% etc in the stock market.

![Capture6](https://user-images.githubusercontent.com/83153124/207227135-5ce25180-178f-4b4f-ac1b-fd5543eb1f19.PNG)

I have also plotted the Box Plot of our dataaset from where we can get more infromation of the volume like the median, min & max, different quartile values etc.

![Capture7](https://user-images.githubusercontent.com/83153124/207227785-385bb568-6fcd-47c9-828a-56c9e4ccc711.PNG)

Then, I have plotted currency VS closing price to get the price information of the cryptocurrencies. For example, in the following image you can see the details information of the Ethereum stock price. And from here we can aso find that though the volume of Tether is very high in the market but it's price is very low compared to Ethereum or Bitcoin.

![Capture8](https://user-images.githubusercontent.com/83153124/207228273-c4638341-7e28-4698-a4f8-eaaf503aa6b1.PNG)

Finally, I have plotted some scattered plots showing the volume compariosns between diffrent currencies during the time period from 2015 to 2020/21.

![Capture9](https://user-images.githubusercontent.com/83153124/207228542-43a25b79-1fdf-494f-9e99-2dce4fa9017f.PNG)

I have also plotted the same graph in logarithmic scale to understand the comparison more precisely.

![Capture10](https://user-images.githubusercontent.com/83153124/207228662-c7cb9d73-e05c-4d8a-958c-2894e76f348b.PNG)

## STEP 5: Addinng new files which have effect of the Bitcoin price
In this step I have added one more dataset where we have some information that have effect on the closing price of the Bitcoin. And in this dataset I have got the information from 2013 to 2018. So, from now on the results I am going to show that are until 2018. Here are the information of some influencers:
- Close: closing price of bitcoin
- btc_market_cap: bitcoin market capitilization for the particular date. Market cap = Total bitcoin volume * price.
- btc_n_transactions_per_block: How many transactions took place per block on a particular date
- abs_btc_count: bitcoin count till date
- btc_hash_rate: Hash rate applied to mine the bitcoins per date
- btc_difficulty: measure of difficulty to mine. The more difficult, the less coins should be mined.
- btc_cost_per_transaction: avg cost of transaction
- btc_n_transactions: # of transactions

## STEP 6 : Understand the Bitcoin price & volume information and how it changes over time
Before going to get the correlation of Bitcoin closing price with influencers, I have analyzed and plotted how the Bitcoin prices and volume changes over time.
When we check the price over years, we can see that there was a sudden spike during 2017/18. The plot shows a huge surge in price of bitcoin in 2017. The price is increased from 1000 to 3000 dollar from earlier 2017 till July 2017 and then from 3000 to 7000 dollars from July to November.

![Capture11](https://user-images.githubusercontent.com/83153124/207229673-ca457658-f13a-445d-9f83-2230ef307a54.PNG)

I have also plotted CandleStick Charts for Financial data visualization.

![Capture13](https://user-images.githubusercontent.com/83153124/207230200-142b3e71-adcb-4804-960b-fa8485ad9d83.PNG)

From the following plot we can see that how the volume of Bitcoin chages during each month. We can see some ups and downs in the volume over time.

![Capture12](https://user-images.githubusercontent.com/83153124/207230008-a42afc73-1f57-45d4-adb2-42d40ee9e3d1.PNG)

And here I have plotted a viloin plot to get some more specific information like median, min & max, different quartile values about the vloume of Bitcoin.

![Capture14](https://user-images.githubusercontent.com/83153124/207230413-c8372893-b922-45d9-8109-d82a3c4539c9.PNG)

## STEP 7: Merging Bitcoin dataset with other data that have effetcs on Bitcoing through 'Date' column
In this step we have merged the othe influencer dataset with the bitcoin dataset according to their date columns. And we also have to do some data preprocessing of the here as the dates were not in same format in two datasets. In the following image you can see that we now have 30columns. So, we have enough influencer information to check whether they have any effect on Bitcoin closing price.

![Capture15](https://user-images.githubusercontent.com/83153124/207231009-a20cd924-fbc4-489b-af6e-38b0f29635b3.PNG)

## STEP 8 : Evaluate Bitcoin closing prices and finding the correlation between the "Closing Price" and other factors that we get from the other dataset
As we are going to get the effetcs on Bitcoin closing price I have first plotted the distribution of closing price of Bitcoin. from here we can see that the lower prices that are close to 1k, in that case it happened several times. However, the maximum price that are arond 20k (until 2018) those were not happeded that much. That means in the maximum price didn't last for that much time.

![Capture16](https://user-images.githubusercontent.com/83153124/207231526-d8d2c844-975d-4f73-bb11-73c1752e98e1.PNG)

I have done the day of week analsysis to find out how the amount of price of Bitcoin effects the closing price of it.

![Capture17](https://user-images.githubusercontent.com/83153124/207232844-1f8d8d62-eeb4-4e8e-9e7a-ca2034d9b8ec.PNG)

The price trend for weekdays is not very clear as it was not in 5 years data plot. But we can still see that:

- In three of five years, Wednesdays see price drops and Mondays see price surge.
- The trend is alternating years is comparable as well. Forexample year 2013, 2015 and 2017 somehow follow the similar trend.

If we look at the mean for day-of-week individually, it seems mean is fluctuating and there is no visible pattern as we saw before. May be price is not a good indicator.

Now, I have tried to find the Bitcoin price correlation with some other variables. We can see the correlation between price and other factors in here.

![Capture18](https://user-images.githubusercontent.com/83153124/207233343-40f235c3-f78f-4656-92ad-3ffa9b342624.PNG)

Since, We are concerned with the relationship between bitcoin and other variables, I have made other values 0 for the sake of clarity.

The map shows that Bitcoin price is most correlated with BTC market capitilization, BTC hash rate and BTC_difficulty.



